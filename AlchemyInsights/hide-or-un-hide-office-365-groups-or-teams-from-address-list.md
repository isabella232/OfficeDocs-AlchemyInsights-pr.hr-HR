---
title: Skrivanje ili poništavanje sakrivanja grupa ili timova sustava Office 365 s popisa adresa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: cb3c2819ff7203774511bd0e45633b59a02091ff
ms.sourcegitcommit: e3a1f96200bc58dc8a5b3597cc2600e71c4bd266
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/14/2020
ms.locfileid: "44225343"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skrivanje ili poništavanje sakrivanja grupa ili timova sustava Office 365 s popisa adresa

Koristite sljedeću naredbu EXO PowerShell da biste sakrili ili poništili skrivanje grupe/timova sustava Office 365 s popisa adresa (GAL) klijenata sustava Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Koristite sljedeću naredbu EXO PowerShell da biste sakrili ili poništili skrivanje grupe/timova sustava Office365 iz klijenata sustava Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Detaljne upute potražite [u odjeljku Skrivanje grupa sustava Office 365 iz gal i klijenata sustava Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
