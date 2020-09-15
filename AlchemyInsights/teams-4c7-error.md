---
title: Pogreška timova 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700195"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 pogreška u Microsoftovim timovima

Ta se pogreška pojavljuje jer Microsoftovi timovi zahtijevaju provjeru autentičnosti obrazaca. Kada implementirate Active Directory Federation Services (AD FS), provjera autentičnosti obrazaca nije omogućena za intranet prema zadanim postavkama. Ako Integrirana provjera autentičnosti sustava Windows ne uspije, od vas će se zatražiti da se prijavite pomoću provjere autentičnosti obrazaca.

Da biste riješili taj problem, omogućite provjeru autentičnosti obrazaca pomoću dodatka AD FS Microsoftova konzola za upravljanje (MMC-a) na računalu koje sadrži lokalnu kopiju servisa Active Directory. Da biste to učinili, slijedite ove korake: 

1. U navigacijskom oknu pronađite **pravila provjere autentičnosti**.
2. U odjeljku **Akcije** u oknu s detaljima odaberite **Uređivanje globalne primarne provjere autentičnosti**.
3. Na kartici **intranetu** odaberite **Provjera autentičnosti obrazaca**.
4. Odaberite **u redu** (ili **Primijeni**).