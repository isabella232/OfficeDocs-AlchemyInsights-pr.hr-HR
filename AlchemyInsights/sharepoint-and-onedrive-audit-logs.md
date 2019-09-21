---
title: Klasična izvješća evidencije nadzornih zapisnika sustava SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068015"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Zapisnici revizije sustava SharePoint i OneDrive

**Dnevnika programa SharePoint i OneDrive moderne jedinstvene revizije iz sukladnosti**

- [Uključi/isključi objedinjeno bilježenje nadzora](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

U sustavu SharePoint ili servisu OneDrive nije potrebna dodatna konfiguracija.

- Korištenje pretraživanja zapisnika nadzora za provjeru aktivnosti datoteka, mapa, korisnika, dozvola:

    - [Aktivnosti datoteka i stranica](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Aktivnosti mape](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Korištenje aktivnosti zahtjeva za dijeljenje i pristup](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Aktivnosti sinkronizacije](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Aktivnosti administracije web-mjesta](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Dodatne informacije o dohvat tih događaja potražite [u pretraživanju zapisnika nadzora](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**SharePoint klasični dnevnici nadzora**

Migrirati SPO naslijeđene revizije na Unified nadzorni zapisnik (UAL). To u biti znači da će se sva bila koja su naslijeđena revizijska izvješća sada moći prenositi preko UAL-a, a naslijeđeni revizijski signali su premješteni u UAL.

Ključne promjene:

- Skraćivanje kao mogućnost nije dostupno.
- Odjeljak u kojem odaberete specifične događaje za reviziju nije dostupan. Molimo pogledajte [ovaj dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) za potpuni popis revidiranih događaja dostupnih prema zadanim postavkama.
- Opcija "lokacija" pod **prilagođenim izvješćima** nije dostupna. 
- Događaji "otvaranje ili preuzimanje dokumenata" nisu dostupni. 

