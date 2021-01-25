---
title: Arhivski poštanski sandučić gotovo je pun
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974211"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Arhivski poštanski sandučić gotovo je pun

Ako korisnik primi upozorenje, **Poštanski sandučić arhive gotovo je pun** ili morate povećati veličinu njihovog arhivskog poštanskog sandučića, evo nekoliko savjeta:

1. Ako je korisniku dodijeljen plan sustava Exchange Online 1, nadogradite ga na licencu za **Exchange Online tarifu 2** da biste povećali veličinu od 50 GB do 100gb.
1. Ako je korisniku već dodijeljen neki od sljedećih načina: **Exchange Online tarifa 2** ili tarifa za Exchange Online 1 s dodacima za arhiviranje sustava Exchange Online, upotrijebite upute u nastavku da biste omogućili automatsko proširenje arhiviranja:.
 
    1. [Spojite se na PowerShell sustava Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Pokrenite sljedeći cmdlet za korisnika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Pokrenite sljedeći cmdlet da biste potvrdili da je omogućen za korisnika:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Dodatne informacije potražite u članku:

- [ Omogućivanje neograničenog arhiviranja-pomoć za administratore – Microsoft 365 sukladnost | Microsoftovi dokumenti](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Ograničenja sustava Exchange Online – opisi servisa | Microsoftovi dokumenti](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Nadogradnja na neki drugi poslovni plan | Microsoftovi dokumenti](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

