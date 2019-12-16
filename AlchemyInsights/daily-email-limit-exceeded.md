---
title: Prekoračeno je svakodnevno ograničenje e-pošte. Tijek rada je suspendiran.
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053109"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dnevna poruka e-pošte premašena. Tijek rada je suspendiran.

Ova pogreška može se primiti u sljedećim scenarijima:

- Imate tijek rada u SharePoint online koji koristi vrstu platforme SharePoint 2010 ili SharePoint 2013 tijek rada.
- Tijek rada je konfiguriran za slanje prilagođene poruke e-pošte na više od 200 korisnika u isto vrijeme, više od 10.000 primatelja po danu ili više od 30 poruka u minuti.
- Kada pokrenete tijek rada, poruka e-pošte nije poslana i primijetite sljedeće ponašanje:
    - Za tijek rada koji koristi vrstu platforme SharePoint 2013, potražite stranicu **status tijeka rada** . Na stranici status tijeka rada, **interni status** je postavljen na **pokretanje**, a informativni balon prikazuje **nemogućnost slanja primatelju**.

Da biste zaobišli taj problem, konfigurirajte tijek rada za slanje poruka e-pošte bez prekoračenja [ograničenja primatelja Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na primjer, koristite pauzu u tijeku rada, pošaljite e-poštu u Office 365 grupu, grupu raspodjele ili sigurnosnu grupu koju je omogućila pošta ili poruku pošaljite manje od 200 primatelja odjednom.


Dodatne informacije potražite u sljedećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Povezane teme
- [Stvori tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 