---
title: Rješavanje Microsoft 365 aplikacija Nažalost, imamo poruku o privremenim problemima s poslužiteljem
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
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021588"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Rješavanje problema Microsoft 365 "Nažalost, imamo privremene probleme s poslužiteljem"

Ako primite ovu poruku, pokušajte sljedeće:

1. Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste potvrdili da ne blokiraju pristup internetu Microsoft 365 aplikacijama. Pogledajte [URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **Pokreni**  >  **pokreni**, a zatim upišite **services.msc**. Provjerite jesu li svi sljedeći servisi pokrenuti:
    - Automatsko postavljanje mrežnih uređaja
    - Servis za mrežni popis
    - Svijesti o mrežnom mjestu
    - Windows Zapisnik događaja

Ako neki od tih servisa nije pokrenut, pokušajte ga pokrenuti. Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu tako da otvorite naredbeni redak s dodatnim dozvolama:

**sfc /scannow**

Kada ova naredba završi, ponovno pokrenite računalo.

Detaljne informacije potražite u članku ["Nažalost, ne možemo se povezati s vašim računom. Kada aktivirate, pokušajte ponovno kasnije".](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)