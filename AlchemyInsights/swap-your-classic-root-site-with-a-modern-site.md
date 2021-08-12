---
title: Zamjena klasičnog korijenskog web-mjesta pomoću modernog web-mjesta
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940811"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamjena klasičnog korijenskog web-mjesta pomoću modernog web-mjesta

Ako je vaše okruženje postavljeno prije travnja 2019., korijensko web-mjesto možete promijeniti u moderno web-mjesto pomoću komponente Microsoft PowerShell:

- Ako imate drugo web-mjesto koje želite koristiti kao korijensko web-mjesto, korijensko web-mjesto možete zamijeniti [(zamijeniti).](https://docs.microsoft.com/sharepoint/modern-root-site) 
    - Koristite [SPOSiteSwap da biste mjesto web-mjesta](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zamijenili drugim web-mjestom prilikom arhiviranja izvornog web-mjesta. Dostupno za timski web-mjesto (nije povezano s grupom) i komunikacijsko web-mjesto. 

- Uskoro će se uvesti dodatne mogućnosti koje će vam omogućiti da nastavite koristiti sadržaj na web-mjestu, ali pretvorite postojeće web-mjesto u komunikacijsko web-mjesto. 
>[!Important]
>Te će se mogućnosti postupno uvaljati. Nastavite provjeravati ima li ažuriranja u centru za poruke. 

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi sa zamjenom web-mjesta

- Ciljno web-mjesto može kratko vrijeme vratiti pogrešku "nije pronađeno" (HTTP 404).
- Da biste ažurirali indeks pretraživanja, morat ćete ponovno stišati sadržaj. Nije potreban ručni korak – to će se učiniti automatski.
- Sve što ovisi o "statičnih" vezama (kao što su sinkronizacija datoteka i OneNote datoteka) morat će se ručno ispraviti.
- Ako je izvorišno web-mjesto bilo web-mjesto s vijestima tvrtke ili ustanove, ažurirajte URL. Nabavite popis svih web-mjesta s vijestima tvrtke ili ustanove.
- Project Možda će biti potrebno provjeriti valjanost web-mjesta poslužitelja da bi se provjerilo jesu li i dalje pravilno povezana.
