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
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627566"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Upravljanje pravilima sastanka u Microsoftovim timovima

Pravila sastanka koriste se za kontrolu značajki koje su dostupne sudionicima koji ispunjavaju sastanke koje su zakazali korisnici u vašoj organizaciji. Neke značajke politika sastanka možda neće biti implementirane u centru za administraciju timova još uvijek (oni su označeni "uskoro" u dokumentaciji). U tom slučaju, ili ako ste uzimajući pogrešku kao što je "ne možemo ažurirati pravila upravo sada, ali pokušajte ponovno kasnije" u Microsoft Teams centar za administraciju, preporučujemo da koristite PowerShell za stvaranje ili izmjenu pravila sastanka timova. 

Dodatne informacije o pravilima sastanka potražite u sljedećim resursima:

- Da biste saznali više o stvaranju pravila, stvaranju promjena i dodjeljivanju korisnika pravilima, pogledajte [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Da biste napravili promjene pravila pomoću PowerShell cmdlets, pogledajte [timove PowerShell pregled](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Morate koristiti [modul Skype za tvrtke PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) za pravila sastanka timova. 
    - Pregled [*-csteamsmetingpolicy dokumente Cmdletovi](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) za više informacija.

**Napomena:** Može potrajati i do 24 sata da bi promjene politike stupile na snagu za korisnike. Možda nećete moći odmah mijenjati novostvorene politike; čekati 4 sata i ponovno pokušati izmijeniti novostvorena pravila. Ako još uvijek imate problema, pokušajte PowerShell.  