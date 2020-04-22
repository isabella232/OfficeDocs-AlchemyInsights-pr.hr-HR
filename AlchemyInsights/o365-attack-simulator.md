---
title: 2681 Napadač simulator u Microsoft 365
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
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713458"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulator napada u sustavu Microsoft 365

- Nedostaje li ti simulator napada? Attack Simulator zahtijeva **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** ili **Office 365 Enterprise E5**. Attack Simulator **nije** obuhvaćen Tarifom za zaštitu od 1 (ATP plan 1), Office 365 Enterprise E3 ili pretplatom na Microsoft 365 za tvrtke.

- Račun koji koristite za pokretanje simuliranih napada zahtijeva dozvole globalnog administratora ili administratora sigurnosti i višestruku provjeru autentičnosti (MFA). Dodatne informacije o preduvjetima attack simulatora potražite [u ovoj temi](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Važne stvari koje treba znati o **Brute Force Password** napad simulacije:

  - Ako je ciljnom računu omogućen MFA i lozinka je ispravno postavljena, račun se neće prikazati kao kompromitiran (drugi faktor provjere autentičnosti bit će nepotpun).

  - Datoteka lozinke ne može biti veća od 10 MB. Upotrijebite jednu lozinku po retku i uključite prazan redak (povratak vagona) nakon zadnje lozinke na popisu.

- Važne stvari koje treba znati o **Spear Phishing** priložiti simulacije:

  - Prema dizajnu, ne možete pružiti prilagođenu vrijednost za **URL poslužitelja za prijavu od krađe identiteta**.

  - Ako primatelj koristi [dodatak Omogući poruku izvješća](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) da bi prijavio poruku kao krađu identiteta, možda nećete primiti upozorenja za poruku (jer je to simulirani napad).

- Izvješća: nakon dovršetka simuliranog napada možete kliknuti **Detalji o napadu** da biste vidjeli izvješće.

- Detaljne upute i nove značajke u attack simulatoru potražite [u odjeljku Attack Simulator u sustavu Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
