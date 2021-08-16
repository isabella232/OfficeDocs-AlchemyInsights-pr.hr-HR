---
title: Teams 4c7
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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049300"
---
# <a name="4c7-error-in-microsoft-teams"></a>Pogreška 4c7 u Microsoft Teams

Ta se pogreška pojavljuje jer Microsoft Teams provjere autentičnosti obrazaca. Prilikom implementacije servisa Active Directory Federation Services (AD FS), provjera autentičnosti obrazaca po zadanom nije omogućena za intranet. Ako Windows provjera autentičnosti ne uspije, od vas će se zatražiti da se prijavite pomoću provjere autentičnosti obrazaca.

Da biste riješili taj problem, omogućite provjeru autentičnosti obrazaca pomoću alata AD FS Microsoft Management Console (MMC) na računalu koje sadrži lokalnu kopiju servisa Active Directory. Da biste to učiniti, slijedite ove korake: 

1. U navigacijskom oknu idite na Pravila **provjere autentičnosti**.
2. U **odjeljku Akcije** u oknu s detaljima **odaberite Uređivanje globalne primarne provjere autentičnosti**.
3. Na kartici **Intranet odaberite** Provjera **autentičnosti obrazaca**.
4. Odaberite **U** redu (ili **Primijeni).**