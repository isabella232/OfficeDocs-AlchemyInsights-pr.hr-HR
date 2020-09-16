---
title: 1491-pretraživanje-ne-vraća-očekuje-Rezultati
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740466"
---
# <a name="content-search-not-returning-expected-results"></a>Pretraživanje sadržaja ne vraća očekivane rezultate

Kada pokrenete pretraživanje sadržaja iz centra za & sigurnost sustava Microsoft 365, možda će vam se prikazati neočekivan rezultat pretraživanja. Razmotrite sljedeće stavke koje mogu utjecati na rezultate pretraživanja:

- **Mjesta sadržaja i uvjeti pretraživanja**: Provjerite jeste li odabrali odgovarajuće lokacije sadržaja i uvjete pretraživanja. Ako ste pokrenuli veliko pretraživanje (s mnogo mjesta), razmotrite njegovo razdvajanje u više pretraživanja.

- **Djelomično indeksirane stavke**:  [djelomično indeksirane stavke](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) iz poštanskih sandučića uvršteni su u procijenjene rezultate pretraživanja. Međutim, djelomično indeksirane stavke s web-mjesta u sustavu SharePoint i OneDrive nisu uključene u procjenu pretraživanja.

- Pogreške u **pretraživanju**: Kada pretražujete veliki broj poštanskih sandučića (iznad 100.000 poštanskih sandučića), možda će vam se prilikom pretraživanja pojavljuje pogreška u pretraživanju uz šifre pogrešaka kao što su CS008-009 i CS012-002). U ovom slučaju ponovno pokušajte pretraživati samo za neuspjela mjesta sadržaja. Dodatne informacije potražite u  [ovom članku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
