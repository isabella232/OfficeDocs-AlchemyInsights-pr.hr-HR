---
title: 2681 simulator napada u sustavu Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506730"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulator napada u sustavu Microsoft 365

- Nedostaje li vam simulator napada? Za simulator napada potreban je **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** ili **Office 365 Enterprise E5**. Simulator napada **nije** obuhvaćen office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 ili bilo koje Aplikacije microsoft 365 za tvrtke pretplate.

- Račun koji koristite za pokretanje simuliranih napada zahtijeva globalne administratorske dozvole ili administratorske dozvole za sigurnost i višestruku provjeru autentičnosti (MFA). Dodatne informacije o zahtjevima attack simulatora potražite [u ovoj temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Važne stvari koje treba znati o **Brute Force Lozinka** napad simulacije:

  - Ako ciljni račun ima omogućen MFA i lozinka je ispravno pogodila, račun se neće prikazati kao ugrožen (drugi faktor provjere autentičnosti će biti nepotpun).

  - Datoteka lozinke ne može biti veća od 10 MB. Upotrijebite jednu lozinku po retku i uključite prazan redak (prijevoz povratak) nakon zadnje lozinke na popisu.

- Važne stvari koje treba znati o **Spear Phishing** priložiti simulacije:

  - Po dizajnu ne možete navesti prilagođenu vrijednost za URL poslužitelja za **prijavu za phishing**.

  - Ako primatelj koristi [dodatak Omogući poruku izvješća](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) da bi prijavio poruku kao krađu identiteta, možda nećete primiti upozorenja za poruku (jer je to simulirani napad).

- Izvješća: nakon dovršetka simuliranog napada možete kliknuti **Detalji napada** da biste vidjeli izvješće.

- Detaljne upute i nove značajke u aplikaciji Attack Simulator potražite u [odjeljku Simulator napada u sustavu Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
