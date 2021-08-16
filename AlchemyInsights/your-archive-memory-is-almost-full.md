---
title: Vaš je arhivski poštanski sandučić gotovo pun
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046744"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Vaš je arhivski poštanski sandučić gotovo pun

Ako korisnik primi upozorenje; **Arhivski poštanski sandučić gotovo je pun** ili morate povećati veličinu poštanskog sandučića arhive, evo nekoliko savjeta:

1. Ako je korisniku dodijeljena Exchange Online Plan 1, nadogradite **na Exchange Online plan 2** da biste povećali veličinu od 50 GB na 100 GB.
1. Ako je korisniku već dodijeljeno nešto od sljedećeg: **Exchange Online Plan 2** ili plan Exchange Online Plan 1 pomoću dodatka Exchange Online arhiviranje, slijedite korake u nastavku da biste omogućili automatsko arhiviranje:.
 
    1. [Povezivanje na Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Pokrenite sljedeći naredbeni redak za korisnika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Pokrenite sljedeću naredbu da biste potvrdili da je korisnik omogućen:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Dodatne informacije potražite u sljedećem članku:

- [Omogućivanje neograničenog arhiviranja – pomoć za administratore – Microsoft 365 usklađenost | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online ograničenja – opisi servisa | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Nadogradnja na drugi poslovni plan | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

