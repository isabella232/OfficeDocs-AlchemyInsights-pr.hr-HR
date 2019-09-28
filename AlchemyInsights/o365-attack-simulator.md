---
title: 2681 napad simulator u Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305324"
---
# <a name="attack-simulator-in-office-365"></a>Napad simulator u Office 365

- Da li ti nedostaje simulator napada? Napad simulator zahtijeva **Office 365 napredni plan zaštite prijetnji 2 (ATP plan 2)** ili **Office 365 Enterprise E5**. Simulator napada nije **uključen u** Office 365 napredni plan zaštite prijetnji 1 (ATP plan 1), Office 365 Enterprise E3 ili bilo koje Office 365 poslovne pretplate.

- Račun koji koristite za pokretanje simulirane napade zahtijeva globalne administratorske ili sigurnosne administratorske dozvole i multi-faktor autentikacije (MFP). Dodatne informacije o zahtjevima simulator napada pogledajte [ovu temu](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Važne stvari koje morate znati o **brutalnoj sile lozinke** napada simulacije:

  - Ako ciljni račun ima MFA omogućen i lozinka je pogodio ispravno, račun neće prikazati kao ugrožen (drugi faktor provjere autentičnosti će biti nepotpun).

  - Datoteka lozinke ne može biti veća od 10 MB. Upotrijebite jednu lozinku po retku i uključite praznu liniju (povratni prijevoz) nakon posljednje lozinke na popisu.

- Važne stvari za znati o **koplja phishing** priložiti simulacije:

  - Po dizajnu, ne možete pružiti prilagođenu vrijednost za **URL poslužitelja za prijavu krađe identiteta**.

  - Ako primatelj koristi [Omogući dodatak poruka izvještaja](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) da bi prijavio poruku kao krađu identiteta, možda nećete primiti upozorenja za poruku (jer je to simulirani napad).

- Izvješća: nakon što je simulirani napad dovršen, možete kliknuti **napad detalji** da biste vidjeli izvješće.

- Za detaljne upute i nove značajke u napad simulator, pogledajte [napad simulator u Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
