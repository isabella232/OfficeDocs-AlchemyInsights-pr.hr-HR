---
title: 2681 simulator napada u programu Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801543"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulator napada u programu Microsoft 365

- Jeste li propustili Attack simulator? Simulator napada zahtijeva **Microsoft Defender za office 365 tarifu 2 (ATP plan 2)** ili **Office 365 Enterprise E5** . Simulator napada nije **sadržan** u programu Microsoft Defender za Office 365 tarifu 1 (ATP plan 1), Office 365 Enterprise E3 ili bilo koje Microsoftove pretplate za tvrtke Microsoft 365.

- Račun koji koristite za pokretanje simuliranih napada zahtijeva globalne dozvole za administratore ili bezbednosne administratore te multi-Factor provjeru autentičnosti (MFA). Dodatne informacije o preduvjetima za simulator napada potražite u [ovoj temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Važne informacije o **brutalnosti napada lozinka** za napade:

  - Ako je ciljni račun omogućen za MFA, a lozinka je ispravno pogađala, račun se neće prikazati kao kompromitiran (drugi faktor provjere autentičnosti bit će nepotpun).

  - Datoteka lozinke ne može biti veća od 10 MB. Koristite jednu lozinku po retku i uvrstite prazni redak (povrat u prijevozu) nakon posljednje lozinke na popisu.

- Važne informacije koje se odnose na **krađu identiteta** priložite simulacije:

  - Prema dizajnu ne možete pružiti prilagođenu vrijednost za **URL poslužitelja za prijavu krađe identiteta** .

  - Ako primatelj koristi dodatak za [poruku izvješća](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) da bi prijavio poruku kao krađu identiteta, možda nećete primati upozorenja za poruku (jer je to simulirani napad).

- Izvješća: nakon dovršetka simuliranog napada možete kliknuti **Detalji o napadu** da biste vidjeli izvješće.

- Detaljne upute i nove značajke u simulatoru Attack potražite [u članku simulator napada u programu Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
