---
title: Smjernice za performanse opće migracije
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
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932471"
---
# <a name="general-migration-performance-guidance"></a>Smjernice za performanse opće migracije

**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokreću poslovne ključne aplikacije na servis koji se izvodi u pozadini. To obuhvaća migraciju sadržaja, sprječavanje gubitka podataka (DLP) i rješenja za sigurnosno kopiranje. Tijekom tih presedana poduzimamo korake da bi servisi sustava SharePoint Online i servisi OneDrive ostali iznimno raspoloživi i pouzdani za korisnike koji više nego ikad ovise o servisu u udaljenim radnim scenarijima.

Na temelju podrške tog cilja implementirali smo čvršća restriktivna ograničenja na pozadinske aplikacije (migracija, DLP i rješenja sigurnosnih kopija) tijekom radnog dana. Trebali biste očekivati da će te aplikacije tijekom tog vremena doseći ograničen protok. No tijekom večeri i vikenda u regiji servis će biti spreman za obradu znatno većeg volumena zahtjeva iz pozadinske aplikacije.

**Smjernice za performanse migracije**

Na performanse migracije mogu utjecati mrežna infrastruktura, veličina datoteke, vrijeme migracije te ograničavanje. Razumijevanje gore navedenog olakšat će vam planiranje i maksimiziranje efikasnosti migracije.

- [Smjernice za performanse opće migracije](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
