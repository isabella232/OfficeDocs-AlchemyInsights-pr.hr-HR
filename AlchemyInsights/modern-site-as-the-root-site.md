---
title: Moderna stranica kao root stranice
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054694"
---
# <a name="modern-site-as-root-site"></a>Moderna stranica kao root stranice

Započeli smo s uvođenju nove značajke koja će vam omogućiti da [zamijenite svoje klasično web-mjesto root stranicu s modernim stranicama](https://docs.microsoft.com/sharepoint/modern-root-site). Pomoću poziva [-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zamijenite mjesto web-mjesta s drugim web-mjestom dok arhivirate originalno web-mjesto. Dostupno i za timsko web-mjesto (nije povezano s grupom) i web-mjesto komunikacije.

>[!Important]
> Nemojte brisati klasični root web stranice za stvaranje moderne komunikacijske stranice. Microsoft ne podržava to. Brisanjem korijenskog web-mjesta sve će SharePoint web-mjesta u vašoj organizaciji biti nedostupne svim korisnicima, sve dok ne vratite web-mjesto ili stvorite novo web-mjesto na istom URL-u. Mi ćemo komunicirati ovu značajku putem centra za poruke. Trebali biste očekivati da će značajka biti uključena u vašeg stanara uskoro.

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi s zamjene web-mjesta
- Ciljno web-mjesto može vratiti pogrešku "nije pronađeno" (HTTP 404) u kratkom vremenskom razdoblju.
- Sadržaj će se morati obnoviti za ažuriranje indeksa pretraživanja. Ovdje nije potreban ručni korak, to će biti učinjeno automatski.
- Sve što ovisi o "statičkim" vezama (kao što su datoteka Sync i OneNote datoteke) morat će se ručno ispraviti.
- Možda će biti potrebno provjeriti web-mjesta Project Servera kako bi se osiguralo da su još uvijek ispravno povezane. 
