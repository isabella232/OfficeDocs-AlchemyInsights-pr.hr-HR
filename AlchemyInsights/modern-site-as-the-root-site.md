---
title: Moderna web-mjesta kao korijensko web-mjesto
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232707"
---
# <a name="modern-site-as-root-site"></a>Moderna web-mjesta kao korijensko web-mjesto

Ćemo imati počelo pripremati rollout nove značajke koje će vam omogućuju da zamijeni vaš klasični mjesta korijensko web-mjesto s Moderna web-mjesta. Koristite [Pozovite SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Zamijeni mjesto web-mjesta s drugog web-mjesta vrijeme arhiviranja izvornog web-mjesta. Dostupno za timskog web-mjesta (nije povezano s grupom) i komunikacije web-mjesta. 

>[!Important]
> Brisanje klasični korijensko web-mjesto za stvaranje Moderna komunikacije web-mjesta. Ovo je Microsoft ne podržava. Brisanje korijenskog web-mjesta će napraviti sve SharePoint web-mjestima u vašoj organizaciji nedostupni na sve korisnike dok ne obnovite web-mjesto ili stvorite novo web-mjesto na URL-u istoj. Ćete smo komunikaciji značajka putem centra za poruku. Značajka biti uključen u vaše klijentske uskoro očekivati.

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi s zamjene web-mjesta
- Ciljno mjesto može vratiti "nije pronađen" Pogreška (HTTP 404) za kratkog vremenskog razdoblja.
- Sadržaj će morati biti ponovno pretražiti da radi indeksiranja da biste ažurirali indeks pretraživanja. Postoji bez ručnog korak potreban ovdje, to će učiniti automatski.
- Ništa zavise "statički" veze (poput datoteka sinkronizacije datoteka i OneNote) morat ćete ručno ispraviti.
- Web-mjesta Project Server možda morati provjeriti da biste bili sigurni da su i dalje povezani ispravno. 
