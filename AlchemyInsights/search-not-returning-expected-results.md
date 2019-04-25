---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383827"
---
# <a name="content-search-not-returning-expected-results"></a>Sadržaja nije uputio očekivane rezultate pretraživanja

Prilikom izvođenja pretraživanja sadržaja iz & Office 365 Sigurnosni centar usklađenosti primiti neočekivani rezultati. Razmotrite sljedeće stvari koje mogu utjecati na rezultate pretraživanja:

- **Mjesta sadržaja i uvjete pretraživanja**: Provjerite ste odabrali odgovarajući mjesta sadržaja i uvjete pretraživanja. Ako ste pokrenuli veliki pretraživanja (s mnogih mjesta), razmislite o podjele u više pretraživanja.

- **Djelomično indeksirane stavke**: [djelomično indeksirane stavke](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) poštanske sandučiće su uključeni u rezultatima pretraživanja procijenjeni. Međutim, djelomično indeksirane stavke s mjesta u SharePoint i OneDrive nisu uključeni u procjenu pretraživanja.

- **Pretraživanje neuspjeha**: prilikom pretraživanja velik broj poštanski sandučići (više od 100 000 poštanske sandučiće), možda ćete dobiti pogreške pretraživanja s kodovi pogreške kao što su CS008 009 i CS012 002). U tom slučaju, ponovno pretraživanje samo za mjesta sadržaja nije uspjelo. Pogledajte [Ovaj članak](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) dodatne informacije.
