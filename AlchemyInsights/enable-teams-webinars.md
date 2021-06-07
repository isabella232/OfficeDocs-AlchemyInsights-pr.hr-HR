---
title: Omogućivanje Teams web-seminara
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793548"
---
# <a name="enable-teams-webinars"></a>Omogućivanje Teams web-seminara

Web-seminari su po zadanom omogućeni. Možete upravljati tko može zakazati i registrirati Teams web-seminare pomoću naredbi Teams PowerShell.

- Svi korisnici koji mogu stvoriti sastanak mogu stvoriti i sastanak web-seminara. Ako želite upravljati tko može zakazati Teams, koristite *AllowMeetingRegistration*. 
- *WhoCanRegister po zadanom je* omogućen i postavljen na **Svi**. Ako želite isključiti registraciju sastanka, *postavite AllowMeetingRegistration na* **False**.

Da biste promijenili te postavke, morate instalirati [Teams PowerShell](/microsoftteams/teams-powershell-install). Pravila sastanka primjenjuju se i na web-seminare Teams sastanaka. Ako je, primjerice, anonimno uključivanje isključeno u postavkama sastanka, anonimni korisnici ne mogu se pridružiti webinarima.

Dodatne informacije o konfiguriranju osoba koje se mogu registrirati za webinare potražite u članku [Konfiguriranje osoba koje se mogu registrirati za webinare](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Dodatne informacije o postavkama za Microsoftove popise potražite u članku [Postavke kontrole za Microsoftove popise](/sharepoint/control-lists).