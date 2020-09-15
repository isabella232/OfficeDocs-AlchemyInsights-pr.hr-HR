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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666862"
---
# <a name="modern-site-as-root-site"></a>Moderno web-mjesto kao korijensko web-mjesto

Započeli smo s prikazom nove značajke koja će vam dopustiti da [zamijenite svoje klasično korijensko web-mjesto s modernim web](https://docs.microsoft.com/sharepoint/modern-root-site)-mjestom. Pomoću poziva [-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) mijenjate mjesto web-mjesta s drugim web-mjestom tijekom arhiviranja izvornog web-mjesta. Dostupno za obje timsko web-mjesto (nije povezano s grupom) i komunikacijskim web-mjestom.

>[!Important]
> Nemojte brisati klasično korijensko web-mjesto da biste stvorili moderno komunikacijsko web-mjesto. Microsoft ne podržava ovo. Brisanjem korijenskog web-mjesta svi će web-mjesta sustava SharePoint u vašoj tvrtki ili ustanovi biti nedostupne svim korisnicima dok ne vratite web-mjesto ili stvorite novo web-mjesto na istom URL-u. Ovu značajku Komunicirat ćemo putem centra za poruke. Morate očekivati da će značajka uskoro biti uključena u zakupcu.

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi s zamjenom web-mjesta
- Odredišno web-mjesto može u kratkom vremenskom periodu vratiti pogrešku "nije pronađeno" (HTTP 404).
- Sadržaj će se morati ponovno vratiti da bi se ažurirao indeks pretraživanja. Ovdje nije potreban ručni korak, to će se obaviti automatski.
- Sve što ovisi o "statički" vezama (kao što su sinkronizacija datoteka i datoteke programa OneNote) morat će se ručno ispraviti.
- Web-mjesta projektnog poslužitelja možda će se morati potvrditi da bi se osiguralo da su i dalje ispravno povezani. 
