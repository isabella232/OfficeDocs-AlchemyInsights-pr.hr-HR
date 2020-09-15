---
title: Klasični Izvještaji zapisnika nadzora sustava SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662200"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Zapisnici nadzora sustava SharePoint i servisa OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Zapisi o reviziji sustava SharePoint Classic

SPO nasljeđeni nadzor migrirao je u jedinstveni zapisnik nadzora (UAL). Sva će se SPO naslijeđena izvješća o reviziji sada powered putem UAL-a, a nasljeđene revizijske signale migrirali su u UAL.

Ključne promjene:

* Podrezivanje nije dostupno kao mogućnost.
* Odabir određenih događaja za reviziju nije dostupan. Pogledajte [ovaj dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) radi potpunog popisa događaja koji se revidiraju na raspolaganju po zadanom.
* Mogućnost **mjesta** u odjeljku **Prilagođena izvješća** nije dostupna.
* Mogućnost **otvaranja ili preuzimanja dokumenata** nije dostupna.

[Konfiguriranje postavki nadzora za zbirku web-mjesta](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Moderno objedinjene zapisnike nadzora sustava SharePoint i OneDrive iz usklađenosti

* [Uključivanje/isključivanje objedinjenog nadzornog zapisivanja](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

U sustavu SharePoint ili na servisu OneDrive nije potrebna nijedna dodatna konfiguracija.

Pomoću pretraživanja zapisnika nadzora potražite aktivnost datoteka, mapa, korisnika, dozvola:

* [Aktivnosti datoteka i stranica](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Aktivnosti u mapama](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Zajedničko korištenje i pristup aktivnostima zahtjeva](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Aktivnosti sinkronizacije](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktivnosti administracije web-mjesta](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Dodatne informacije o dohvat tih događaja potražite [u članku pretraživanje zapisnika nadzora](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
