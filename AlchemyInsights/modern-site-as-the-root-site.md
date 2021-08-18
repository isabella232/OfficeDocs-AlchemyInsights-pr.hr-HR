---
title: Moderno web-mjesto kao korijensko web-mjesto
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327594"
---
# <a name="modern-site-as-root-site"></a>Moderno web-mjesto kao korijensko web-mjesto

Počeli smo s uvođenjem nove značajke koja će vam omogućiti zamjenu klasičnog korijenskog web-mjesta [s modernim web-mjestom](https://docs.microsoft.com/sharepoint/modern-root-site). Koristite [SPOSiteSwap za zamjenu mjesta web-mjesta](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) s drugim web-mjestom prilikom arhiviranja izvornog web-mjesta. Dostupno za timski web-mjesto (nije povezano s grupom) i komunikacijsko web-mjesto.

**Važno:** nemojte izbrisati klasično korijensko web-mjesto da biste stvorili moderno komunikacijsko web-mjesto. Microsoft to ne podržava. Brisanjem korijenskog web-mjesta svi će SharePoint web-mjesta u vašoj tvrtki ili ustanovi biti nedostupni svim korisnicima dok ne vratite web-mjesto ili stvorite novo web-mjesto na istom URL-u. Tu ćemo značajku komunicirati putem centra za poruke. Trebali biste očekivati da će značajka uskoro biti uključena u klijentu.

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi sa zamjenom web-mjesta
- Ciljno web-mjesto može kratko vrijeme vratiti pogrešku "nije pronađeno" (HTTP 404).
- Da biste ažurirali indeks pretraživanja, morat ćete ponovno stišati sadržaj. Ovdje nije potreban ručni korak, to će se učiniti automatski.
- Sve što ovisi o "statičnih" vezama (kao što su sinkronizacija datoteka i OneNote datoteka) morat će se ručno ispraviti.
- Project Možda je potrebno provjeriti valjanost web-mjesta poslužitelja da bi se provjerilo jesu li i dalje pravilno povezana. 
