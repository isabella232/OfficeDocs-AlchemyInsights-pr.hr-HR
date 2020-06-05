---
title: Aktivacija Issue - Nismo u mogućnosti to povezivanje odmah
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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581867"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Popravljanje poruke aplikacije Microsoft 365 "Trenutno se ne možemo povezati"

Ako primite ovu poruku, pokušajte sljedeće:

1. Provjerite postavke vatrozida, antivirusnog softvera i proxy poslužitelja da biste potvrdili da ne blokiraju pristup internetu aplikacijama sustava Microsoft 365. Pogledajte [Microsoftove URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **Pokreni**  >  **,** a zatim upišite **services.msc**. Provjerite jesu li pokrenuti sljedeći servisi:
    - Automatsko postavljanje uređaja povezanih s mrežom
    - Usluga mrežnog popisa
    - Svijest o mrežnom mjestu
    - Zapisnik događaja sustava Windows

Ako jedan od tih servisa nije pokrenut, pokušajte ga pokrenuti. Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog retka s povišenim dozvolama:

**sfc / scannow**

Nakon što ova naredba završi, ponovo pokrenite računalo.

Detaljne informacije potražite u [odjeljku "Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije" pogreška kada aktivirate Office iz Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).