---
title: Učvršćivanje Officeovih aplikacija Žao mi je, imamo privremenu poruku o problemima poslužitelja
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627982"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Popravljanje aplikacija sustava Office "Žao mi je, imamo privremene probleme s poslužiteljem"

Ako primite ovu poruku, pokušajte sljedeće:

1. Provjerite vatrozid, antivirusni softver i postavke proxyja da biste potvrdili da ne blokiraju pristup internetu aplikacijama sustava Office. Pogledajte [Office 365 URL-ove i IP adrese raspona](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **pokretanje** > **, a**zatim upišite **Services. msc**. Provjerite jesu li sve sljedeće usluge pokrenite:
    - Automatsko podešavanje uređaja povezanih s mrežom
    - Servis popisa mrežnih usluga
    - Svijest o mrežnom mjestu
    - Zapisnik događaja u sustavu Windows

Ako jedna od tih usluga nije pokrenut, pokušajte ga pokrenuti. Ako imate problem s započinjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog retka s povišenim dozvolama:

**sfc/scannow**

Nakon završetka ove naredbe, ponovo pokrenite računalo.

Detaljne informacije potražite u stranici ["Žao mi je, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije "pogreška kada aktivirate Office iz Officea 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).