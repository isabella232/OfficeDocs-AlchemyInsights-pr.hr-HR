---
title: 1491-search-not-returning-očekivani rezultati
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709219"
---
# <a name="content-search-not-returning-expected-results"></a>Pretraživanje sadržaja ne vraća očekivane rezultate

Prilikom pokretanja pretraživanja sadržaja iz centra za sigurnost sustava Microsoft 365 & centru za usklađenost, možda ćete dobiti neočekivane rezultate pretraživanja. Razmotrite sljedeće stvari koje mogu utjecati na rezultate pretraživanja:

- **Lokacije sadržaja i uvjeti pretraživanja:** Provjerite jeste li odabrali odgovarajuće lokacije sadržaja i uvjete pretraživanja. Ako ste pokrenuli veliko pretraživanje (s mnogo lokacija), razmislite o podjeli u više pretraživanja.

- **Djelomično indeksirane stavke**: [Djelomično indeksirane stavke](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) iz poštanskih sandučića uključene su u procijenjene rezultate pretraživanja. Međutim, djelomično indeksirane stavke s web-mjesta u sustavu SharePoint i OneDrive nisu uključene u procjenu pretraživanja.

- **Pogreške u pretraživanju**: Prilikom pretraživanja velikog broja poštanskih sandučića (više od 100 000 poštanskih sandučića) možete dobiti pogreške pretraživanja s kodovima pogrešaka kao što su CS008-009 i CS012-002). U tom slučaju ponovno pokušajte pretraživati samo za neuspjela mjesta sadržaja. Dodatne informacije potražite [u ovom članku.](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)
