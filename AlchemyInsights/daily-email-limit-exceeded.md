---
title: Premašeno je dnevno ograničenje e-pošte. Tijek rada obustavljen.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059631"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dnevni e-pošta Premašeno ograničenje. Tijek rada obustavljen.

Ova se pogreška možda primili u sljedećim scenarijima:

- Imate tijeka rada u SharePoint Online koji koriste SharePoint 2010 ili vrsta platformi SharePoint 2013 tijeka rada.
- Tijek rada konfiguriran za slanje poruka e-pošte prilagođenih više od 200 korisnicima na vrijeme, više od 10 000 primatelja po danu ili na više od 30 poruka u minuti.
- Kada pokrenete tijek rada, poruka e-pošte nije poslana i primijetiti sljedeće ponašanje:
    - Za tijek rada pomoću vrsta platformi SharePoint 2013 pregledavati stranicu **Stanje tijeka rada** . Na stranici Stanje tijeka rada **Interna Status** postavljen u **pokrenuto**i prikazuje balončić informacije **nije bilo moguće poslati primatelju**.

Da biste zaobišli taj problem, konfigurirajte tijeka rada za slanje poruka e-pošte bez Prekoračenje [ograničenja Exchange Online pošiljatelja](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Ako, na primjer, koristiti zaustavljanje u tijeku rada, slanje e-pošte grupi Office 365, grupu raspodjele ili pošte omogućeno sigurnosne grupe ili poslati poruku manje od 200 primateljima odjednom.


Za dodatne informacije pogledajte sljedeći [članak](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Povezane teme
- [Stvaranje toka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i tijek](https://flow.microsoft.com/blog/sharepoint-and-flow/) 