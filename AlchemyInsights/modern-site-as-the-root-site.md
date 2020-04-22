---
title: Moderna stranica kao root site
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713783"
---
# <a name="modern-site-as-root-site"></a>Moderna stranica kao root site

Počeli smo uvesti novu značajku koja će vam omogućiti da [zamijenite svoje klasične stranice root stranice s modernim stranicama](https://docs.microsoft.com/sharepoint/modern-root-site). Koristite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) za zamjenu lokacije web-mjesta s drugim web-mjestom dok arhivijete izvornu web-lokaciju. Dostupno za timsko web-mjesto (nije povezano s grupom) i komunikacijskom web-mjestu.

>[!Important]
> Nemojte brisati svoje klasične root stranice za stvaranje moderne komunikacijske stranice. Microsoft to ne podržava. Brisanjem korijenskog web-mjesta sva sharepoint web-mjesta u tvrtki ili ustanovi neće biti dostupna svim korisnicima dok ne vratite web-mjesto ili stvorite novo web-mjesto na istom URL-u. Ovu ćemo značajku komunicirati putem centra za poruke. Uskoro biste trebali očekivati da će značajka biti uključena u klijentu.

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi s adut za zamjenu web-mjesta
- Ciljno web-mjesto može vratiti pogrešku "nije pronađeno" (HTTP 404) na kratko vrijeme.
- Sadržaj će se morati preistovjetnuti radi ažuriranja indeksa pretraživanja. Ovdje nije potreban ručni korak, to će se učiniti automatski.
- Sve što ovisi o "statičkim" vezama (kao što su Sinkronizacija datoteka i onenote datoteka) morat će se ručno ispraviti.
- Možda će biti potrebno provjeriti valjanost web-mjesta sustava Project Server da bi se osiguralo da su još uvijek ispravno pridružena. 
