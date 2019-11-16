---
title: Pristup uslugama umirovljenja
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747776"
---
# <a name="access-services-retirement"></a>Pristup uslugama umirovljenja

Kao što smo prvotno najavili u MC97576, u ožujku 2017, i nastavio komunicirati tijekom protekle godine Accessove usluge su umirovljene iz Office 365. Sljedeća faza u ovom procesu će biti uklanjanje Access web baze podataka koje koriste SharePoint popise kao njihove temeljne pohrane podataka.

**Kako to utječe na mene?**

Počevši od lipnja 2019, zaustavit ćemo stvaranje novih baza podataka programa Access u sustavu SharePoint online i isključiti uslugu i sve preostale aplikacije do travnja 2020.

**Što trebam učiniti kako bih se pripremio za ovu promjenu?**

Potičemo vas da stvorite plan prijelaza za web-baze podataka programa Access vaše organizacije. Administratori mogu koristiti [skener aplikacije SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) za dobivanje inventara aplikacija programa Access koje web-mjesta koriste.

Postoji nekoliko načina Migriranje podataka web-baze programa Access:

- Uvoz u lokalnu bazu podataka programa Access (. ACCDB) ili u Excelovu datoteku.
- Preporučujemo i istraživanje Microsoft PowerApps kao alternativne platforme za stvaranje nekôda poslovnih rješenja za web i mobilne uređaje.