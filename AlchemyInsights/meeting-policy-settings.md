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
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376556"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Upravljanje pravilima sastanka u Microsoftovim timovima

Pravila sastanka koriste se za kontrolu značajki koje su dostupne sudionicima koji ispunjavaju sastanke koje su zakazali korisnici u vašoj organizaciji. Neke značajke politika sastanka možda neće biti implementirane u centru za administraciju timova još uvijek (oni su označeni "uskoro" u dokumentaciji). U tom slučaju, ili ako ste uzimajući pogrešku kao što je "ne možemo ažurirati pravila upravo sada, ali pokušajte ponovno kasnije" u Microsoft Teams centar za administraciju, preporučujemo da koristite PowerShell za stvaranje ili izmjenu pravila sastanka timova. 

Dodatne informacije o pravilima sastanka potražite u sljedećim resursima:

- Da biste saznali više o stvaranju pravila, stvaranju promjena i dodjeljivanju korisnika pravilima, pogledajte [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Da biste napravili promjene pravila pomoću PowerShell cmdlets, pogledajte [timove PowerShell pregled](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Morate koristiti [modul Skype za tvrtke PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) za pravila sastanka timova. 
    - Pregled [*-csteamsmetingpolicy dokumente Cmdletovi](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) za više informacija.

**Napomena:** Može potrajati i do 24 sata da bi promjene politike stupile na snagu za korisnike. Možda nećete moći odmah mijenjati novostvorene politike; čekati 4 sata i ponovno pokušati izmijeniti novostvorena pravila. Ako još uvijek imate problema, pokušajte PowerShell.  