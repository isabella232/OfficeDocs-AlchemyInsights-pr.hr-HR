---
title: Klasična izvješća zapisnika nadzora sustava SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509592"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Zapisnici nadzora sustava SharePoint i OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Klasični zapisnici nadzora sustava SharePoint

Naslijeđeno nadziranje SPO-a migrirao je u Objedinjeni zapisnik nadzora (UAL). Sva SPO naslijeđena revizijska izvješća sada će se pokretati putem UAL-a, a naslijeđeni revizijski signali migrirali su u UAL.

Ključne promjene:

* Podrezivanje nije dostupno kao mogućnost.
* Odabir određenih događaja za reviziju NIJE dostupan. Pogledajte [ovaj dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) za potpuni popis revidiranih događaja dostupnih prema zadanim postavkama.
* Mogućnost **Lokacija** u **odjeljku Prilagođena izvješća** nije dostupna.
* Mogućnost **Otvaranje ili preuzimanje događaja dokumenata** NIJE dostupna.

[Konfiguriranje postavki nadzora za zbirku web-mjesta](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Zapisnici sustava SharePoint i OneDrive modernog objedinjenog nadzora iz usklađenosti

* [Uključivanje/isključivanje objedinjenog zapisivanja nadzora](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

U sustavu SharePoint ili OneDrive nije potrebna dodatna konfiguracija.

Koristite pretraživanje zapisivanja nadzora da biste provjerili aktivnost datoteka, mapa, korisnika, dozvola:

* [Aktivnosti datoteka i stranica](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Aktivnosti mape](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Dijeljenje i pristup aktivnosti zahtjeva](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Aktivnosti sinkronizacije](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktivnosti administracije web-mjesta](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Dodatne informacije o dohvaćanju tih događaja potražite [u odjeljku Pretraživanje zapisnika nadzora](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
