---
title: Prepoznavanje IP adrese i klijenta u zapisnikima nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716380"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Prepoznavanje IP adrese i klijenta u zapisnikima nadzora

IP adresa koja odgovara aktivnosti korisnika ili administratora sustava Microsoft 365 prikazana je u zapisnikima nadzora. Podaci o klijentu također su prijavljeni. Evo koraka za utvrđivanje takvih informacija

1. Prijavite se u Centar za [sigurnost sustava Microsoft 365 & .](https://protection.office.com/)

2. Idite na stranicu **za** > **pretraživanje zapisnika nadzora** pretraživanja.

   Ako ste zainteresirani za određenu aktivnost, odaberite je s popisa **Aktivnosti.** Ako nije, sve aktivnosti bit će vraćene za odabranog korisnika (zadana postavka).

   **Napomena**: Određene aktivnosti možda neće biti dostupne u izborniku **Aktivnosti;** međutim, te će stavke nadzora biti vraćene ako je **odabrana mogućnost Prikaži rezultate za sve aktivnosti** (zadana postavka).

3. Navedite korisničko ime u polju **Korisnici,** odaberite odgovarajući datumski raspon aktivnosti, a zatim kliknite **Pretraži**.

U rezultatima možete vidjeti IP adresu za tu aktivnost u oknu s rezultatima. Odaberite zapis nadzora da biste vidjeli detaljne informacije u potpaleti **Detalji** (na primjer, Klijent, Korisnik koji je izvršio akciju itd.).

Dodatne informacije [potražite u odjeljku Pronalaženje IP adrese računala koje se koristi za pristup ugroženom računu](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
