---
title: Očekivani rezultati za 1491-search-not-returning
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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510564"
---
# <a name="content-search-not-returning-expected-results"></a>Pretraživanje sadržaja ne vraća očekivane rezultate

Prilikom pokretanja pretraživanja sadržaja iz centra za usklađenost & sustava Microsoft 365, možda ćete primiti neočekivane rezultate pretraživanja. Razmotrite sljedeće stvari koje mogu utjecati na rezultate pretraživanja:

- **Lokacije sadržaja i uvjeti pretraživanja**: Provjerite jeste li odabrali odgovarajuće lokacije sadržaja i uvjete pretraživanja. Ako ste pokrenuli veliko pretraživanje (s mnogo lokacija), razmislite o tome da ga podijelite u više pretraživanja.

- **Djelomično indeksirane stavke**: [Djelomično indeksirane stavke](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) iz poštanskih sandučića uključene su u procijenjene rezultate pretraživanja. Međutim, djelomično indeksirane stavke s web-mjesta u sustavima SharePoint i OneDrive nisu uključene u procjenu pretraživanja.

- **Pogreške u pretraživanju**: prilikom pretraživanja velikog broja poštanskih sandučića (više od 100 000 poštanskih sandučića), možda ćete dobiti pogreške pretraživanja s kodovima pogrešaka kao što su CS008-009 i CS012-002). U tom slučaju pokušajte potražiti samo za neuspjele lokacije sadržaja. Dodatne informacije potražite u [ovom članku.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)
