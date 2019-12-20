---
title: Ekipa 4c7 pogreška
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796008"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 pogreška u Microsoftovim timovima

Ta se pogreška pojavljuje jer Microsoft Teams zahtijeva provjeru autentičnosti obrazaca. Kada implementirati Active Directory Federation Services (AD FS), provjera autentičnosti obrazaca nije omogućena za intranet prema zadanim postavkama. Ako Integrirana provjera autentičnosti sustava Windows ne uspije, zatražit će se da se prijavite pomoću provjere autentičnosti obrazaca.

Da biste riješili taj problem, omogućite provjeru autentičnosti obrazaca pomoću dodatka AD FS Microsoftova konzola za upravljanje (MMC) na računalu s lokalnom kopijom servisa Active Directory. Da biste to učinili, slijedite ove korake: 

1. U navigacijskom oknu pregledajte **pravila provjere autentičnosti**.
2. U odjeljku **Akcije** u oknu s detaljima odaberite **Uređivanje globalne primarne provjere autentičnosti**.
3. Na kartici **intraneta** odaberite **provjeru autentičnosti obrazaca**.
4. Odaberite **u redu** (ili **Primijeni**).