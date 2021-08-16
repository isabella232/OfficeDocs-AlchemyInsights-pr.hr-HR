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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000378"
---
# <a name="modern-site-as-root-site"></a>Moderno web-mjesto kao korijensko web-mjesto

Počeli smo s uvođenjem nove značajke koja će vam omogućiti zamjenu klasičnog korijenskog web-mjesta [s modernim web-mjestom](https://docs.microsoft.com/sharepoint/modern-root-site). Koristite [SPOSiteSwap da biste mjesto web-mjesta](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zamijenili drugim web-mjestom prilikom arhiviranja izvornog web-mjesta. Dostupno za timski web-mjesto (nije povezano s grupom) i komunikacijsko web-mjesto.

>[!Important]
> Nemojte izbrisati klasično korijensko web-mjesto da biste stvorili moderno komunikacijsko web-mjesto. Microsoft to ne podržava. Brisanjem korijenskog web-mjesta svi će SharePoint web-mjesta u vašoj tvrtki ili ustanovi učiniti nedostupnima svim korisnicima dok ne vratite web-mjesto ili stvorite novo web-mjesto na istom URL-u. Tu ćemo značajku komunicirati putem centra za poruke. Trebali biste očekivati da će značajka uskoro biti uključena u klijentu.

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi sa zamjenom web-mjesta
- Ciljno web-mjesto može kratko vrijeme vratiti pogrešku "nije pronađeno" (HTTP 404).
- Da biste ažurirali indeks pretraživanja, morat ćete ponovno stišati sadržaj. Ovdje nije potreban ručni korak, to će se učiniti automatski.
- Sve što ovisi o "statičnih" vezama (kao što su sinkronizacija datoteka i OneNote datoteka) morat će se ručno ispraviti.
- Project Možda će biti potrebno provjeriti valjanost web-mjesta poslužitelja da bi se provjerilo jesu li i dalje pravilno povezana. 
