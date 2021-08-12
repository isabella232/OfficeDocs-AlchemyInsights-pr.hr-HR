---
title: Prekoračuje se dnevno ograničenje e-pošte. Tijek rada je obustavljen.
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914643"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Prekoračuje se dnevno ograničenje e-pošte. Tijek rada je obustavljen.

Ta se pogreška može primiti u sljedećim scenarijima:

- U web-aplikaciji SharePoint Online imate tijek rada koji koristi vrstu platforme SharePoint 2010 ili SharePoint 2013.
- Tijek rada konfiguriran je tako da prilagođenu poruku e-pošte šalje više od 200 korisnika, više od 10 000 primatelja dnevno ili više od 30 poruka u minuti.
- Kada pokrenete tijek rada, poruka e-pošte ne šalje se i primijetit ćete sljedeće ponašanje:
    - Tijek rada koji koristi vrstu platforme SharePoint 2013 potražite na stranici **Stanja tijeka** rada. Na stranici Stanje tijeka rada **interni status** postavljen je na **Pokrenuto**, a informativni balončić prikazuje **Nije moguće poslati primatelju**.

Da biste zaobišli taj problem, konfigurirajte tijek rada tako da šalje poruke e-pošte bez [prekoračenja ograničenja Exchange Online pošiljatelja](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Primjerice, koristite pauzu u tijeku rada, pošaljite poruku e-pošte u grupu Microsoft 365, grupu za raspodjelu ili sigurnosnu grupu s omogućenom poštom ili pošaljite poruku manje od 200 primatelja istovremeno.


Dodatne informacije potražite u sljedećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Povezane teme
- [Stvaranje Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 