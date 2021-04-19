---
title: Skrivanje i skrivanje grupa ili timova sustava Office 365 s popisa adresa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811448"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skrivanje i skrivanje grupa ili timova sustava Office 365 s popisa adresa

Pomoću sljedeće naredbe exo PowerShell sakrijte ili ne sakrijte grupu/timove sustava Office 365 s popisa adresa (GAL) klijenata sustava Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Pomoću sljedeće naredbe exo PowerShell sakrijte ili de-sakrijte grupu/timove sustava Office365 iz klijenata sustava Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Detaljne upute potražite u članku [Sakrivanje grupa sustava Office 365 iz klijenata sustava GAL i sustava Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
