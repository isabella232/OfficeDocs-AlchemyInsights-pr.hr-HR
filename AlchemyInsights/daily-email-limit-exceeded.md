---
title: Premašeno je dnevno ograničenje e-pošte. Tijek rada je obustavljen.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908696"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Premašilo je dnevno ograničenje e-pošte. Tijek rada je obustavljen.

Ova pogreška može se primiti u sljedećim scenarijima:

- Imate tijek rada u sustavu SharePoint Online koji koristi vrstu platforme tijeka rada sustava SharePoint 2010 ili SharePoint 2013.
- Tijek rada konfiguriran je za slanje prilagođene poruke e-pošte većem broju od 200 korisnika odjednom, više od 10 000 primatelja dnevno ili više od 30 poruka u minuti.
- Kada pokrenete tijek rada, poruka e-pošte se ne šalje i primijetite sljedeće ponašanje:
    - Za tijek rada koji koristi vrstu platforme Sustava SharePoint 2013 potražite stranicu **Stanja tijeka rada.** Na stranici Stanja tijeka rada **interno je stanje** postavljeno na **Pokrenuto**, a oblačić s informacijama prikazuje **nije moguće poslati primatelju**.

Da biste zaobišli taj problem, konfigurirajte tijek rada za slanje poruka e-pošte bez prekoračenja [ograničenja pošiljatelja sustava Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na primjer, koristite pauzu u tijeku rada, pošaljite e-poštu grupi microsoft 365, grupi za raspodjelu ili sigurnosnoj grupi omogućenoj za poštu ili pošaljite poruku manje od 200 primatelja odjednom.


Dodatne informacije potražite u sljedećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Povezane teme
- [Stvori tijek](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 