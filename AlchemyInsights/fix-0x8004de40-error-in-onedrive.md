---
title: Ispravite pogreške 0x8004de40 u OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755840"
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