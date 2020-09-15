---
title: Mirovina u programu Access Services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698638"
---
# <a name="access-services-retirement"></a>Mirovina u programu Access Services

Kao što smo prvobitno najavili u MC97576, u ožujku 2017, i nastavili smo komunicirati u prošloj godini programa Access Services su u mirovini. Sljedeća faza u ovom postupku bit će uklanjanje web-baza podataka programa Access koja koristi popise sustava SharePoint kao njihovo spremište podataka u pozadini.

**Kako to utječe na mene?**

Počevši od lipnja 2019, zaustavit ćemo stvaranje novih baza podataka programa Access u sustavu SharePoint online i isključivanje servisa i svih preostalih aplikacija do travnja 2020.

**Što je potrebno učiniti da biste se pripremili za ovu promjenu?**

Preporučujemo vam da stvorite plan tranzicije za web-baze podataka programa Access tvrtke ili ustanove. Administratori mogu koristiti [skener aplikacija sustava SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) da bi nabavili inventar aplikacija programa Access koje koriste web-mjesta.

Podaci za web-baze podataka programa Access mogu se migrirati na nekoliko načina:

- Uvoz u lokalnu bazu podataka programa Access (. ACCDB) ili u datoteku programa Excel.
- Preporučujemo i istraživanje Microsoft PowerApps kao alternativne platforme za stvaranje nekodova poslovnih rješenja za web i mobilne uređaje.