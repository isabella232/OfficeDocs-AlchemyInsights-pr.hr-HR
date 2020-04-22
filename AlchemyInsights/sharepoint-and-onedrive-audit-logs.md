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
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741957"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Zapisnici nadzora sustava SharePoint i OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Klasični zapisnici nadzora sustava SharePoint

SPO naslijeđeno nadziranje premješteno je u zapisnik objedinjenog nadzora (UAL). Sva spovita izvješća o reviziji SPO-a sada će biti napajana putem UAL-a, a naslijeđeni revizijski signali migrirani su u UAL.

Ključne promjene:

* Podrezivanje NIJE dostupno kao sposobnost.
* Odabir određenih događaja za reviziju NIJE dostupan. Pogledajte [ovaj dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) za potpuni popis nadziranih događaja dostupnih prema zadanim postavkama.
* Mogućnost **Lokacija** u **odjeljku Prilagođena izvješća** NIJE dostupna.
* Mogućnost Otvaranje ili preuzimanje događaja **dokumenata** NIJE dostupna.

[Konfiguriranje postavki nadzora za zbirku web-mjesta](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Datoteke s objema nadzora sustava SharePoint i OneDrive iz usklađenosti

* [Uključivanje/isključivanje objedinjenog zapisivanja nadzora](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Nije potrebna dodatna konfiguracija u sustavu SharePoint ili OneDrive.

Koristite pretraživanje zapisivanja nadzora da biste provjerili aktivnost datoteka, mapa, korisnika, dozvola:

* [Aktivnosti datoteka i stranica](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Aktivnosti mapa](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Dijeljenje i pristup aktivnostima zahtjeva](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Aktivnosti sinkronizacije](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktivnosti administracije web-mjesta](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Dodatne informacije o dohvaćanju tih događaja [potražite u odjeljku Pretraživanje zapisnika nadzora](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
