---
title: Performanse migracije sustava ShairPoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931883"
---
# <a name="sharepoint-migration-performance"></a>Performanse migracije sustava ShairPoint

**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokreću poslovne ključne aplikacije na servis koji se izvodi u pozadini. To obuhvaća migraciju sadržaja, sprječavanje gubitka podataka (DLP) i rješenja za sigurnosno kopiranje. Tijekom tih presedana poduzimamo korake da bi servisi sustava SharePoint Online i servisi OneDrive ostali iznimno raspoloživi i pouzdani za korisnike koji više nego ikad ovise o servisu u udaljenim radnim scenarijima.

Na temelju podrške tog cilja implementirali smo čvršća restriktivna ograničenja na pozadinske aplikacije (migracija, DLP i rješenja sigurnosnih kopija) tijekom radnog dana. Trebali biste očekivati da će te aplikacije tijekom tog vremena doseći ograničen protok. No tijekom večeri i vikenda u regiji servis će biti spreman za obradu znatno većeg volumena zahtjeva iz pozadinske aplikacije.

**Performanse migracije**

Na performanse migracije mogu utjecati mrežna infrastruktura, veličina datoteke, vrijeme migracije te ograničavanje. Razumijevanje gore navedenog olakšat će vam planiranje i maksimiziranje efikasnosti migracije.

Da biste saznali više, posjetite poveznice u nastavku.

- [SharePoint Online i brzina ODB migracije](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [Izbjegavanje uskih grla ili blokiranja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [Preuzimanje i instalacija alata za migraciju sustava SharePoint](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
