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
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825435"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Upravljanje pravilima sastanka u aplikaciji Microsoft Teams

**Napomena: korisnicima može trebati do 24 sata da promjene pravilnika stupe na snagu.** Možda nećete moći odmah mijenjati novostvorene pravilnike. pričekajte 4 sata i pokušajte ponovno izmijeniti novostvoreni pravilnik.

Pravila sastanka koriste se za kontrolu značajki koje su dostupne sudionicima sastanka za sastanke koje zakazali korisnici u vašoj tvrtki ili ustanovi. Neke značajke pravilnika za sastanke možda se još neće implementirati u centru za administratore aplikacije Teams (one su u dokumentaciji označene kao "uskoro"). U tom slučaju ili ako vam se prikazuje pogreška kao što je "Trenutno ne možemo ažurirati pravilnik, ali ga kasnije pokušati ponovno" u centru za administratore aplikacije Microsoft Teams, preporučujemo da pomoću komponente PowerShell stvorite ili izmijenite pravilnike za sastanke servisa Teams. 

Dodatne informacije o pravilima sastanka potražite u sljedećim resursima:

- Informacije o stvaranju pravilnika, unošanju promjena i dodjeljivanju korisnika pravilniku pogledajte u članku Upravljanje [pravilnikom za sastanke u aplikaciji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Da biste unijeli promjene pravilnika pomoću cmdleta komponente PowerShell, pogledajte [pregled komponente Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Morate koristiti modul [PowerShell skypea za tvrtke za pravilnike](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) sastanka aplikacije Teams. 
    - Dodatne informacije [potražite u dokumentaciji cmdleta *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

