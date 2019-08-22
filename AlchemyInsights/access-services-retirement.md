---
title: Access services umirovljenje
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495743"
---
# <a name="access-services-retirement"></a>Access services umirovljenje

Kao smo izvorno najavio u MC97576, u 2017 Ožujak i nastavlja komunikaciju putem prošle godine Access Services u mirovini su se iz Office 365. Sljedeće faze ovaj proces će biti uklanjanje pristup web-baze podataka koje koriste SharePoint popise kao njihove podlozi pohranu podataka.

**Kako to utječe na mene?**

Početni lipanj 2019 ćemo će zaustaviti stvaranje nove baze podataka programa Access u SharePoint Online i isključi servis i sve preostale apps po 2020 Travanj.

**Što je potrebno učiniti da biste pripremili za ovu promjenu?**

Pozivamo vas da stvorite plan tranzicije za vaša organizacija pristup web-baze podataka. Administratori možete koristiti [pristup SharePoint app skener](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) da biste nabavili zaliha apps pristup koji koriste web-mjesta.

Postoji nekoliko načina za migraciju podataka Access web baze podataka:

- Uvoz lokalne baze podataka Access (. ACCDB) ili datoteku programa Excel.
- Preporučujemo i istraživanje Microsoft PowerApps kao alternativni platforma za stvaranje rješenja bez koda poslovne za web i mobilnih uređaja.