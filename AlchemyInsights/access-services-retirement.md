---
title: Access services umirovljenje
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769429"
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