---
title: Rješavanje problema s aplikacijom Microsoft 365 Nažalost, imamo poruku o privremenim problemima s poslužiteljem
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835263"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Popravljanje aplikacije Microsoft 365 "Nažalost, imamo privremene probleme s poslužiteljem"

Ako primite ovu poruku, pokušajte sljedeće:

1. Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste potvrdili da ne blokiraju pristup internetu aplikacijama Microsoft 365. Pogledajte [URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **Pokreni**  >  **pokreni**, a zatim upišite **services.msc**. Provjerite jesu li svi sljedeći servisi pokrenuti:
    - Automatsko postavljanje mrežnih uređaja
    - Servis za mrežni popis
    - Svijesti o mrežnom mjestu
    - Zapisnik događaja u sustavu Windows

Ako neki od tih servisa nije pokrenut, pokušajte ga pokrenuti. Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu tako da otvorite naredbeni redak s dodatnim dozvolama:

**sfc /scannow**

Kada ova naredba završi, ponovno pokrenite računalo.

Detaljne informacije potražite u članku ["Nažalost, ne možemo se povezati s vašim računom. Kada aktivirate, pokušajte ponovno kasnije".](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)