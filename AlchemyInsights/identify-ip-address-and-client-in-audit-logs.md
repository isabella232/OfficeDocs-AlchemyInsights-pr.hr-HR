---
title: Prepoznavanje IP adrese i klijenta u zapisnicima nadzora
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
ms.openlocfilehash: 080b3df3934781ebf0d0cd5243787bf6975fc5f123b5b1593c0b6d9ada4eae5d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887492"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Prepoznavanje IP adrese i klijenta u zapisnicima nadzora

IP adresa koja odgovara aktivnosti korisnika Microsoft 365 administratora prikazuje se u zapisnicima nadzora. Zapisuje se i podaci o klijentu. U nastavku su navedene upute za prepoznavanje takvih podataka

1. Prijavite se u [centar za Microsoft 365 usklađenost](https://protection.office.com/).

2. Idite na stranicu **pretraživanje**  >  **zapisnika nadzora pretraživanja.**

   Ako vas zanima određena aktivnost, odaberite je na **popisu** Aktivnosti. Ako ne, sve će se aktivnosti vratiti za odabranog korisnika (zadana postavka).

   **Napomena:** određene aktivnosti možda neće biti dostupne na **izborniku** Aktivnosti; No te će se stavke nadzora vratiti ako je **odabrana postavka** Prikaži rezultate za sve aktivnosti (zadana postavka).

3. Navedite korisničko ime u **polju** Korisnici, odaberite odgovarajući raspon datuma za aktivnost, a zatim kliknite **Pretraži**.

U rezultatima možete vidjeti IP adresu za tu aktivnost u oknu s rezultatima. Odaberite zapis nadzora da  biste vidjeli detaljne informacije u letku Detalji (na primjer, Klijent, Korisnik koji je izveo akciju itd.).

Dodatne informacije potražite u članku [Pronalaženje IP adrese računala koje se koristi za pristup ugroženom računu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
