---
title: Prepoznavanje IP adresa i klijenta u evidenciji nadzora
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668302"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Prepoznavanje IP adresa i klijenta u evidenciji nadzora

IP adresa koja odgovara aktivnosti korisnika sustava Microsoft 365 ili administratora prikazuje se u evidenciji nadzora. Prijavljeni su i podaci o klijentu. Evo koraka za identifikaciju takvih informacija

1. Prijavite se u [centar za sigurnost & sustava Microsoft 365](https://protection.office.com/).

2. Idite na stranicu **Search**  >  **pretraživanja zapisnika nadzora** pretraživanja.

   Ako ste zainteresirani za određenu aktivnost, odaberite je na popisu **aktivnosti** . Ako ne, sve će se aktivnosti vratiti odabranom korisniku (zadana postavka).

   **Pažnja**: određene aktivnosti možda neće biti dostupne na izborniku **aktivnosti** ; No te će se stavke u reviziji vratiti ako je odabrano **Prikaz rezultata za sve aktivnosti** (zadana postavka).

3. Navedite korisničko ime u polju **korisnici** , odaberite odgovarajući raspon datuma za aktivnost, a zatim kliknite **Pretraži**.

U rezultatima možete vidjeti IP adresu za tu aktivnost u oknu rezultata. Odaberite zapis nadzora da biste vidjeli detaljne informacije u nastavku za **detalje** (na primjer, klijent, korisnik koji je izvršio akciju, itd.).

Dodatne informacije potražite u članku [Pronalaženje IP adrese računala koje se koristi za pristup kompromitiranom računu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
