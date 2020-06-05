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
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580325"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Premašeno je dnevno ograničenje e-pošte. Tijek rada je obustavljen.

Ta se pogreška može primiti u sljedećim scenarijima:

- Imate tijek rada u sustavu SharePoint Online koji koristi vrstu platforme tijeka rada sustava SharePoint 2010 ili SharePoint 2013.
- Tijek rada konfiguriran je za slanje prilagođene poruke e-pošte više od 200 korisnika odjednom, više od 10.000 primatelja dnevno ili više od 30 poruka u minuti.
- Kada pokrenete tijek rada, poruka e-pošte se ne šalje i primijetite sljedeće ponašanje:
    - Tijek rada pomoću vrste platforme sustava SharePoint 2013 potražite stranicu **Stanja tijeka rada.** Na stranici Stanje tijeka rada **interni status** postavljen je na **Pokrenuto,** a oblačik s informacijama prikazuje **Nije moguće poslati primatelju**.

Da biste zaobiљli taj problem, konfigurirajte tijek rada za slanje poruka e-pošte bez prekoračenja [granica poљiljatelja sustava Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na primjer, koristite pauzu u tijeku rada, pošaljite e-poštu grupi Microsoft 365, grupi za raspodjelu ili sigurnosnoj grupi s omogućenom poštom ili pošaljite poruku manjem od 200 primatelja odjednom.


Dodatne informacije potražite u sljedećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Povezane teme
- [Stvori tijek](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 