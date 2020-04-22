---
title: Popravljanje aplikacija sustava Office Nažalost, imamo poruku o privremenim problemima s poslužiteljem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764109"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Učvršćivanje poruka "Nažalost, imamo privremene probleme s poslužiteljem"

Ako primite ovu poruku, pokušajte sljedeće:

1. Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste potvrdili da ne blokiraju pristup internetu aplikacijama sustava Office. Pogledajte [URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **Pokreni** > **,** a zatim upišite **services.msc**. Provjerite jesu li pokrenuti sljedeći servisi:
    - Automatsko postavljanje mrežnih povezanih uređaja
    - Usluga popisa mreža
    - Svijest o mrežnom mjestu
    - Zapisnik događaja u sustavu Windows

Ako se jedna od tih usluga ne izvodi, pokušajte ga pokrenuti. Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog retka s povišenim dozvolama:

**sfc / scannow**

Nakon dovršetka ove naredbe ponovo pokrenite računalo.

Detaljne informacije potražite u [odjeljku "Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije" pogreška prilikom aktivacije](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).