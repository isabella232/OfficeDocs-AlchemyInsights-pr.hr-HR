---
title: Prepoznavanje IP adrese i klijenta u zapisnicima nadzora
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
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508908"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Prepoznavanje IP adrese i klijenta u zapisnicima nadzora

IP adresa koja odgovara aktivnosti korisnika ili administratora sustava Microsoft 365 prikazana je u zapisnicima nadzora. Podaci o klijentu također su prijavljeni. Evo koraka za utvrđivanje takvih informacija

1. Prijavite se u Centar za [usklađenost sa sigurnosnim & sustava Microsoft 365](https://protection.office.com/).

2. Idite **Search**na  >  stranicu za pretraživanje**zapisnika nadzora** pretraživanja.

   Ako vas zanima određena aktivnost, odaberite je na popisu **Aktivnosti.** Ako nije, sve aktivnosti bit će vraćene za odabranog korisnika (zadana postavka).

   **Napomena**: Određene aktivnosti možda neće biti dostupne u izborniku **Aktivnosti;** međutim, te stavke nadzora vratit će se ako je **odabrana prikazana prikazuje rezultata za sve aktivnosti** (zadana postavka).

3. Navedite korisničko ime u polju **Korisnici,** odaberite odgovarajući datumski raspon aktivnosti, a zatim kliknite **Pretraži**.

U rezultatima možete vidjeti IP adresu za tu aktivnost u oknu rezultata. Odaberite zapis nadzora da biste vidjeli detaljne informacije u potpaleti **Detalji** (na primjer, Klijent, Korisnik koji je izvršio akciju itd.).

Dodatne informacije [potražite u odjeljku Pronalaženje IP adrese računala koje se koristi za pristup kompromitiranom računu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
