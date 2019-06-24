---
title: Ispravite pogreške 0x8004de40 u OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133969"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Ispravite pogreške 0x8004de40 u OneDrive

Ako primite poruku o pogrešci 0x8004de40 s OneDrive:

- Ponovo pokrenite problematično računalo dok ste povezani s aktinvo direktorij domene.
- Ako ponovno pokretanje ne riješi problem, odvajanja od i ponovno se pridružite uređaj iz Azure AD. 

**Napomena**: treba biti na mreži tvrtke prilikom izvođenja ove korake. Ne izvršite ove kada niste moći povezati s korporacijskom Infrastruktura (na primjer, tijekom putovanja). 

- Otvorite privilegiranom naredbenom retku. 
- Da biste otvorili privilegirani naredbeni redak, kliknite - **Start**, desnom tipkom miša kliknite **naredbeni redak**i zatim kliknite **Pokreni kao administrator**.
- Upišite *dsregcmd /leave* i pritisnite **Enter**.
- Kada je dovršeno, upišite *dsregcmd /join* i pritisnite tipku **Enter**.
- Kad je dovršeno, zatvorite naredbeni redak.
- Ponovno pokrenite računalo i prijavite se u OneDrive.