---
title: Zamijenite svoju klasični root stranicu s modernim stranicama
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042919"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamijenite svoju klasični root stranicu s modernim stranicama

Ako je vaša okolina postavljena prije travnja 2019, možete promijeniti korijensko web-mjesto na moderno web-mjesto pomoću Microsoft PowerShell:

- Ako imate drugo web-mjesto koje želite koristiti kao root web-mjesto, možete zamijeniti [(swap) root web-mjesto](https://docs.microsoft.com/sharepoint/modern-root-site) s njom. 
    - Pomoću poziva [-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zamijenite mjesto web-mjesta s drugim web-mjestom dok arhivirate originalno web-mjesto. Dostupno i za timsko web-mjesto (nije povezano s grupom) i web-mjesto komunikacije. 

- Uskoro će se uvesti dodatne mogućnosti koje će vam omogućiti da nastavite koristiti sadržaj na web-mjestu, ali pretvorite postojeće web-mjesto na web-mjesto komunikacije. 
>[!Important]
>Ove mogućnosti će se postupno isvaljivati. Nastavite provjeriti Office 365 Message Center za ažuriranja. 

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi s zamjene web-mjesta

- Ciljno web-mjesto može vratiti pogrešku "nije pronađeno" (HTTP 404) u kratkom vremenskom razdoblju.
- Sadržaj će se morati obnoviti za ažuriranje indeksa pretraživanja. Nema ručnog koraka potreban-to će biti učinjeno automatski.
- Sve što ovisi o "statičkim" vezama (kao što su datoteka Sync i OneNote datoteke) morat će se ručno ispraviti.
- Ako je izvorna web-lokacija web-mjesta interesne grupe, ažurirajte URL.Nabavite popis svih web-mjesta organizacijskih vijesti.
- Možda će biti potrebno provjeriti web-mjesta Project Servera kako bi se osiguralo da su još uvijek ispravno povezane.





