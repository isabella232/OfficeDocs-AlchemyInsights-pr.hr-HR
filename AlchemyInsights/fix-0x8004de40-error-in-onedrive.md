---
title: Popravak pogreške 0x8004de40 na servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716020"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Popravak pogreške 0x8004de40 na servisu OneDrive

Ako primite poruku o pogrešci 0x8004de40 sa servisom OneDrive:

- Ponovno podizanje sustava izvještačen računalo kratak vremenski razmak povezivanje to tvoj Acitve Imenik domena.
- Ako ponovno pokretanje ne riješi problem, poništite vezu i ponovno se pridružite uređaju iz azure AD-a. 

**Napomena:** Trebali biste biti na svojoj korporativnoj mreži tijekom izvođenja ovih koraka. Nemojte izvoditi ove korake kada se ne možete povezati s vašom poslovnom infrastrukturom (na primjer, tijekom putovanja). 

- Otvorite privilegirani naredbeni redak. 
- Da biste otvorili privilegirani naredbeni redak, kliknite – **Start**, desnom tipkom miša kliknite **Naredbeni redak,** a zatim **kliknite Pokreni kao administrator**.
- Tip *dsregcmd dopust* i prisutan **Ulaziti**.
- Kada završite, upišite *dsregcmd /join* i pritisnite **Enter**.
- Kada završite, zatvorite naredbeni redak.
- Ponovno pokrenite računalo i prijavite se na OneDrive.