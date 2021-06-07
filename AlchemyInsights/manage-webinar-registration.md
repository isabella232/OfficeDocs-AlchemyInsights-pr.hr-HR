---
title: Upravljanje registracijom webinara
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793617"
---
# <a name="manage-webinar-registration"></a>Upravljanje registracijom webinara

Upravljate tko se može registrirati za Teams web-seminare pomoću Teams powershell naredbi. Da biste instalirali Teams PowerShell, [pogledajte Teams PowerShell](/microsoftteams/teams-powershell-install). 

*WhoCanRegister po zadanom je* omogućen i postavljen na **EveryoneInCompany**. Da biste svima, uključujući anonimne korisnike, omogućili registraciju, morate postaviti pravilnik sastanka **svima** pomoću naredbe Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Napomena:** ako je anonimno pridruživanje isključeno u postavkama sastanka, anonimni korisnici ne mogu se uključiti u web-seminare. Dodatne informacije i omogućivanje te postavke potražite u članku [Upravljanje postavkama sastanka Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Ako želite isključiti registraciju sastanka, *postavite AllowMeetingRegistration na* **False**.

Dodatne informacije o konfiguriranju osoba koje se mogu registrirati za webinare potražite u članku [Konfiguriranje osoba koje se mogu registrirati za webinare](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Dodatne informacije o postavkama za Microsoftove popise potražite u članku [Postavke kontrole za Microsoftove popise](/sharepoint/control-lists).
