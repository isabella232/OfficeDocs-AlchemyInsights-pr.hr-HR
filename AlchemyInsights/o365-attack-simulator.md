---
title: 2681 Attack Simulator u Microsoft 365
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
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325063"
---
# <a name="attack-simulator-in-microsoft-365"></a>Napad u Microsoft 365

- Nedostaje li vam simulator napada? U programu Attack Simulator **potreban je Microsoft Defender Office 365 plan 2** ili Office 365 Enterprise **E5**. Simulator napada nije **obuhvaćen** programom Microsoft Defender za Office 365 plan 1, Office 365 Enterprise E3 ni bilo koju Microsoft 365 Apps za male tvrtke pretplate.

- Račun koji koristite za pokretanje simuliranih napada zahtijeva dozvole globalnog administratora ili administratora sigurnosti i višestruku provjeru autentičnosti (MFA). Dodatne informacije o preduvjetima za Napad na simulatoru potražite [u ovoj temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Važne stvari koje je važno znati o **simulacijama** napada lozinkom na silu:

  - Ako je ciljni račun omogućio MFA, a lozinka je pravilno odabrana, račun se neće prikazati kao ugrožen (drugi faktor provjere autentičnosti bit će nepotpun).

  - Datoteka lozinke ne smije biti veća od 10 MB. Upotrijebite jednu lozinku po retku i nakon zadnje lozinke na popisu uvrstjte prazan redak (povrat prijevoza).

- Važne stvari koje je važno znati o krađi **identiteta koplja prilaganje** simulacija:

  - Prema dizajnu ne možete navesti prilagođenu vrijednost ZA URL poslužitelja za prijavu **u krađu identiteta.**

  - Ako primatelj koristi dodatak Omogući poruku izvješća da bi prijavio poruku kao krađu identiteta, možda ne primate upozorenja za poruku (jer je [to](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) simulirani napad).

- Izvješća: kada simulirani napad završi, možete kliknuti Detalji o **napadu da** biste vidjeli izvješće.

- Detaljne upute i nove značajke u programu Attack Simulator potražite u članku [Napad u Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
