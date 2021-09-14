---
title: Izvršavanje ograničenja za primanje poštanskih sandučića
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/31/2021
ms.locfileid: "59315799"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Izvršavanje ograničenja za primanje poštanskih sandučića

Microsoft je nedavno počeo s radom na pragu po poštanskom sandučiću od 3600 poruka po satu. Dodatne informacije potražite u članku [Exchange Online ograničenja](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Microsoft 365 poštanski sandučići koji primaju više od 3600 poruka u roku od sat vremena gase se za sljedećih 60 minuta. 

Osim toga, primjenjuje se ograničenje broja parova pošiljatelja i primatelja (SRP) koje blokira poruke koje Microsoft 365 poštanski sandučić određenog pošiljatelja. Ako jedan pošiljatelj pošalje više od 33 % ukupnog praga ili 1200 poruka po trenutnom satu određenom primatelju, ograničenje SRP-a se otvara, a poštanski sandučić više ne prihvaća poruke tog pošiljatelja. Imajte na umu da:

- To je ograničenje aplikacija za poruke e-pošte primljene od drugih korisnika, lokalnog ili internetskog pošiljatelja.
- Isporuka e-pošte u poštanski sandučić blokirana je sljedećih 60 minuta. 
- Pošiljatelji u te poštanske sandučiće primaju izvješće o neisporuci (5.2.121 ili 5.2.122) u kojem se navodi da je poštanski sandučić prekoračio maksimalni prag isporuke. Intra-klijent (pošta unutar istog klijenta) i dalje se isporučuje.
- Kada se primjenjuje ograničenje SRP-a, poštanski sandučić primatelja i dalje prihvaća poruke drugih pošiljatelja.

Administratori mogu nadzirati trenutnu aktivnost poštanskog sandučića tako da pristupe novom izvješću i uvidu u centar za administratore Exchange naziva "Poštanski sandučići koji premašuju ograničenja primanja". Uvid se prikazuje samo ako klijent ima uvrijediti poštanske sandučiće, dok se izvješće uvijek prikazuje na nadzornoj ploči, ali je prazno ako klijent ne uvrijediti poštanske sandučiće.

Dodatne informacije o ograničenjima primanja uvida potražite u članku Poštanski sandučići koji premašuju uvid u primanje ograničenja [u novom EAC-u.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Dodatne informacije o izvješću o prekoračenju ograničenja primanja potražite u članku Poštanski sandučići koji premašuju izvješće o [ograničenjima primanja u novom EAC-u.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)