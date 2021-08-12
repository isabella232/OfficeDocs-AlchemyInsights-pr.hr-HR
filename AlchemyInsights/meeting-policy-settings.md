---
title: Postavke pravilnika sastanka
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925157"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Upravljanje pravilima sastanka u Microsoft Teams

**Napomena: korisnicima može trebati do 24 sata da promjene pravilnika stupe na snagu.** Možda nećete moći odmah mijenjati novostvorene pravilnike. pričekajte 4 sata i pokušajte ponovno izmijeniti novostvoreni pravilnik.

Pravila sastanka koriste se za kontrolu značajki koje su dostupne sudionicima sastanka za sastanke koje zakazali korisnici u vašoj tvrtki ili ustanovi. Neke značajke pravilnika za sastanke možda se još neće implementirati u centru Teams za administratore (one su u dokumentaciji označene kao "uskoro"). U tom slučaju ili ako vam se prikazuje pogreška kao što je "Trenutno ne možemo ažurirati pravilnik, ali ga kasnije pokušati ponovno" u centru za administratore sustava Microsoft Teams preporučujemo da pomoću komponente PowerShell stvorite ili izmijenite pravilnike Teams sastanka. 

Dodatne informacije o pravilima sastanka potražite u sljedećim resursima:

- Da biste saznali više o stvaranju pravilnika, unošanju promjena i dodjeli korisnika pravilniku, pogledajte upravljanje [pravilnikom za sastanke Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Da biste unijeli promjene pravilnika pomoću cmdleta komponente PowerShell, [Teams pregled ljuske PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Da biste koristili pravilnike [Skype za tvrtke powershell,](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) morate koristiti Teams powershell. 
    - Dodatne informacije [potražite u dokumentaciji cmdleta *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

