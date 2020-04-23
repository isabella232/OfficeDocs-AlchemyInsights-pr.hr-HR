---
title: Zamjena klasičnog korijenskog web-mjesta modernim web-mjestom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741536"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamjena klasičnog korijenskog web-mjesta modernim web-mjestom

Ako je okruženje postavljeno prije travnja 2019., korijensko web-mjesto možete promijeniti na moderno web-mjesto pomoću komponente Microsoft PowerShell:

- Ako imate drugu web-lokaciju koju želite koristiti kao root web-lokaciju, možete zamijeniti [(zamijeniti) korijensku stranicu](https://docs.microsoft.com/sharepoint/modern-root-site) s njom. 
    - Koristite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) za zamjenu lokacije web-mjesta s drugim web-mjestom dok arhivijete izvornu web-lokaciju. Dostupno za timsko web-mjesto (nije povezano s grupom) i komunikacijskom web-mjestu. 

- Uskoro će se uvesti dodatne mogućnosti koje će vam omogućiti da nastavite koristiti sadržaj na web-mjestu, ali pretvorite postojeće web-mjesto na komunikacijsko web-mjesto. 
>[!Important]
>Te će se mogućnosti postupno uvesti. Nastavite provjeravati ima li u centru za poruke ažuriranja. 

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi s adut za zamjenu web-mjesta

- Ciljno web-mjesto može vratiti pogrešku "nije pronađeno" (HTTP 404) na kratko vrijeme.
- Sadržaj će se morati preistovjetnuti radi ažuriranja indeksa pretraživanja. Nema ručnog koraka - to će se učiniti automatski.
- Sve što ovisi o "statičkim" vezama (kao što su Sinkronizacija datoteka i onenote datoteka) morat će se ručno ispraviti.
- Ako je izvorišno web-mjesto bilo organizacijsko web-mjesto za vijesti, ažurirajte URL.Nabavite popis svih organizacijskih web-mjesta s novostima.
- Možda će biti potrebno provjeriti valjanost web-mjesta sustava Project Server da bi se osiguralo da su još uvijek ispravno pridružena.
