---
title: Popravljanje aplikacija sustava Microsoft 365 Nažalost, imamo poruku o privremenim problemima s poslužiteljem
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582695"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Ispravak poruke aplikacije Microsoft 365 "Nažalost, imamo privremene probleme s poslužiteljem"

Ako primite ovu poruku, pokušajte sljedeće:

1. Provjerite postavke vatrozida, antivirusnog softvera i proxy poslužitelja da biste potvrdili da ne blokiraju pristup internetu aplikacijama sustava Microsoft 365. Pogledajte [URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **Pokreni**  >  **,** a zatim upišite **services.msc**. Provjerite jesu li pokrenuti sljedeći servisi:
    - Automatsko postavljanje uređaja povezanih s mrežom
    - Usluga mrežnog popisa
    - Svijest o mrežnom mjestu
    - Zapisnik događaja sustava Windows

Ako jedan od tih servisa nije pokrenut, pokušajte ga pokrenuti. Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog retka s povišenim dozvolama:

**sfc / scannow**

Nakon što ova naredba završi, ponovo pokrenite računalo.

Detaljne informacije potražite u [odjeljku "Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije" pogreška kada aktivirate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).