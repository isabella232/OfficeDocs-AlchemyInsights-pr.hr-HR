---
title: Problem s aktivacijom – trenutno se ne možemo povezati
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716164"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Popravljanje poruke aplikacije sustava Office "Trenutno se ne možemo povezati"

Ako primite ovu poruku, pokušajte sljedeće:

1. Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste potvrdili da ne blokiraju pristup internetu aplikacijama sustava Office. Pogledajte [Microsoftove URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **Pokreni** > **,** a zatim upišite **services.msc**. Provjerite jesu li pokrenuti sljedeći servisi:
    - Automatsko postavljanje mrežnih povezanih uređaja
    - Usluga popisa mreža
    - Svijest o mrežnom mjestu
    - Zapisnik događaja u sustavu Windows

Ako se jedna od tih usluga ne izvodi, pokušajte ga pokrenuti. Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog retka s povišenim dozvolama:

**sfc / scannow**

Nakon dovršetka ove naredbe ponovo pokrenite računalo.

Detaljne informacije potražite u [odjeljku "Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovo kasnije" kada aktivirate Office iz sustava Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).