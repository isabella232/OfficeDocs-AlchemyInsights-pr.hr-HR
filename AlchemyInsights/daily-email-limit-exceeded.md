---
title: Prekoračena je dnevna ograničenje e-pošte. Tijek rada je obustavljen.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731555"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Prekoračena je dnevna ograničenje e-pošte. Tijek rada je obustavljen.

Ta se pogreška može primiti u sljedećim scenarijima:

- Imate tijek rada u sustavu SharePoint online koji koristi vrstu platforme tijeka rada sustava SharePoint 2010 ili SharePoint 2013.
- Tijek rada konfiguriran je za slanje prilagođene poruke e-pošte na više od 200 korisnika istodobno, više od 10.000 primatelja dnevno ili više od 30 poruka po minuti.
- Kada pokrenete tijek rada, poruka e-pošte ne šalje se i primijetit ćete sljedeće ponašanje:
    - Za tijek rada pomoću vrste platforme sustava SharePoint 2013 možete potražiti stranicu **statusa tijeka rada** . Na stranici Stanje tijeka rada, **interni status** postavljen je na **pokrenut**, a balon informacija **ne može se prikazati primatelju**.

Da biste zaobišli taj problem, konfigurirajte tijek rada za slanje poruka e-pošte bez prekoračenja [ograničenja pošiljatelja sustava Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na primjer, koristite pauzu u tijeku rada, pošaljite poruku e-pošte grupi Microsoft 365, grupi za raspodjelu ili sigurnosnoj grupi za e-poštu ili pošaljite poruku na manje od 200 primatelja istodobno.


Dodatne informacije potražite u sljedećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Povezane teme
- [Stvaranje toka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 