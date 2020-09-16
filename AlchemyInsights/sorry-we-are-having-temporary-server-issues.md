---
title: Popravljanje aplikacija Microsoft 365 Žao nam je, ali imamo poruku o privremenim problemima s poslužiteljem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758237"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Rješavanje aplikacija Microsoft 365 "Nažalost, imamo problema s privremenim poslužiteljem"

Ako primite ovu poruku, pokušajte sljedeće:

1. Provjerite vatrozid, antivirusni softver i postavke proxy poslužitelja da biste potvrdili da ne blokiraju pristup internetu u aplikacije Microsoft 365. Pročitajte članak [URL-ovi i rasponi IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **početak**  >  **pokretanja**, a zatim upišite **Services. msc**. Provjerite jesu li svi sljedeći servisi pokrenuti:
    - Automatsko postavljanje mrežnih povezanih uređaja
    - Servis mrežnog popisa
    - Svijest o mrežnom mjestu
    - Zapisnik događaja u sustavu Windows

Ako jedan od tih servisa nije pokrenut, pokušajte ga pokrenuti. Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog upita s dodatnim dozvolama:

**sfc/scannow**

Kada naredba završi, ponovno pokrenite računalo.

Detaljne informacije potražite u članku ["Žao nam je, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije "pogreška prilikom aktivacije](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).