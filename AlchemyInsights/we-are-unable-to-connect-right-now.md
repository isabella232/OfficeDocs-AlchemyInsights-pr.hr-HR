---
title: Problem s aktivacijom – trenutno se ne možemo povezati
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
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998141"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Rješavanje problema Microsoft 365 aplikacije "Trenutno se ne možemo povezati"

Ako primite ovu poruku, pokušajte sljedeće:

1. Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste potvrdili da ne blokiraju pristup internetu Microsoft 365 aplikacijama. Pogledajte [Microsoftove URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **Pokreni**  >  **pokreni**, a zatim upišite **services.msc**. Provjerite jesu li svi sljedeći servisi pokrenuti:
    - Automatsko postavljanje mrežnih uređaja
    - Servis za mrežni popis
    - Svijesti o mrežnom mjestu
    - Windows Zapisnik događaja

Ako neki od tih servisa nije pokrenut, pokušajte ga pokrenuti. Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu tako da otvorite naredbeni redak s dodatnim dozvolama:

**sfc /scannow**

Kada ova naredba završi, ponovno pokrenite računalo.

Detaljne informacije potražite u članku ["Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije" kada aktivirate Office iz Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).