---
title: Fix 0x8004de40 pogreška u servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052029"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40 pogreška u servisu OneDrive

Ako primite pogrešku 0x8004de40 s servisom OneDrive:

- Ponovno pokrenite zahvaćeno računalo dok ste spojeni na svoju domenu Acitve Directory.
- Ako ponovno pokretanje ne popravi problem, nepridružite se i ponovno pridružite uređaju iz servisa Azure AD. 

**Napomena**: trebali biste biti na korporacijskoj mreži tijekom izvođenja ovih koraka. Nemojte obavljati ove korake kada se ne možete povezati s korporativnom infrastrukturom (na primjer, tijekom putovanja). 

- Otvorite povećani naredbeni redak. 
- Da biste otvorili povećani naredbeni redak, kliknite- **Start**, desnom tipkom miša kliknite **naredbeni redak**, a zatim kliknite **Pokreni kao administrator**.
- Upišite *dsregcmd/dopust* i pritisnite **Enter**.
- Kada dovršite, upišite *dsregcmd/Join* i pritisnite **Enter**.
- Kada završite, zatvorite naredbeni redak.
- Ponovno pokrenite računalo i prijavite se na OneDrive.