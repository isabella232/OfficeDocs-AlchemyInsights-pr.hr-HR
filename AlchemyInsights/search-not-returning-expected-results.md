---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052702"
---
# <a name="content-search-not-returning-expected-results"></a>Pretraživanje sadržaja ne vraća očekivane rezultate

Prilikom pokretanja pretraživanja sadržaja iz centra Microsoft 365 sigurnosti & usklađenost, možda ćete dobiti neočekivane rezultate pretraživanja. Razmislite o sljedećim stvarima koje mogu utjecati na rezultate pretraživanja:

- **Mjesta sadržaja i uvjeti pretraživanja**: provjerite jeste li odabrali odgovarajuća mjesta sadržaja i uvjete pretraživanja. Ako ste vodili veliko pretraživanje (s mnogo mjesta), razmislite o tome da ga podijelite na više pretraživanja.

- **Djelomično indeksirane stavke: djelomično**  [indeksirane stavke iz](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) poštanskih sandučića obuhvaćene su procijenjenim rezultatima pretraživanja. No djelomično indeksirane stavke s web-mjesta SharePoint OneDrive nisu obuhvaćene procijenite pretraživanja.

- **Pogreške** pri pretraživanju : prilikom pretraživanja velikog broja poštanskih sandučića (više od 100 000 poštanskih sandučića) mogu se pojaviti pogreške pri pretraživanju s kodovima pogrešaka kao što su CS008-009 i CS012-002). U tom slučaju ponovno pokušajte pretraživati samo mjesta neuspjelog sadržaja. Dodatne  [informacije potražite](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) u ovom članku.
