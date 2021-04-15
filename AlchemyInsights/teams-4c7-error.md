---
title: Pogreška u aplikaciji Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786661"
---
# <a name="4c7-error-in-microsoft-teams"></a>Pogreška 4c7 u aplikaciji Microsoft Teams

Ta se pogreška pojavljuje jer je za Microsoft Teams potrebna provjera autentičnosti obrazaca. Prilikom implementacije servisa Active Directory Federation Services (AD FS), provjera autentičnosti obrazaca po zadanom nije omogućena za intranet. Ako integrirana provjera autentičnosti u sustavu Windows ne uspije, od vas će se zatražiti da se prijavite pomoću provjere autentičnosti obrazaca.

Da biste riješili taj problem, omogućite provjeru autentičnosti obrazaca pomoću alata AD FS Microsoft Management Console (MMC) na računalu koje sadrži lokalnu kopiju servisa Active Directory. Da biste to učiniti, slijedite ove korake: 

1. U navigacijskom oknu idite na Pravila **provjere autentičnosti**.
2. U **odjeljku Akcije** u oknu s detaljima **odaberite Uređivanje globalne primarne provjere autentičnosti**.
3. Na kartici **Intranet odaberite** Provjera **autentičnosti obrazaca**.
4. Odaberite **U** redu (ili **Primijeni).**