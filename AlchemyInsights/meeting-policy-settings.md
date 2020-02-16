---
title: Postavke pravila sastanka
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042836"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Upravljanje pravilima sastanka u microsoft teams

**Napomena: može potrajati i do 24 sata da promjene pravila stupe na snagu za korisnike.** Možda nećete moći odmah izmijeniti novostvorena pravila; pričekajte 4 sata i pokušajte ponovno izmijeniti novostvorena pravila.

Pravila sastanka koriste se za kontrolu značajki dostupnih sudionicima sastanka za sastanke koje su zakazali korisnici u vašoj tvrtki ili ustanovi. Neke značajke pravila sastanka možda se još neće implementirati u centru za administratore sustava Teams (one su uskoro označene kao "uskoro" u dokumentaciji). U tom slučaju ili ako vam se prikaže pogreška kao što je "Ne možemo ažurirati pravila odmah, ali pokušajte ponovno kasnije" u centru za administratore sustava Microsoft Teams, preporučujemo da koristite PowerShell za stvaranje ili izmjenu pravila sastanka sustava Teams. 

Dodatne informacije o pravilima sastanka potražite u sljedećim resursima:

- Da biste saznali više o stvaranju pravila, unosenju promjena i dodjeli korisnika pravilima, pročitajte odjeljko [Upravljanje pravilima sastanka u sustavu Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Da biste promijenili pravila pomoću cmdleta komponente PowerShell, pogledajte [pregled komponente Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Morate koristiti [modul PowerShell servisa Skype za tvrtke](https://www.microsoft.com/download/details.aspx?id=39366) za pravilniko o sastanku sustava Teams. 
    - Dodatne informacije potražite u [dokumentaciji cmdleta *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

