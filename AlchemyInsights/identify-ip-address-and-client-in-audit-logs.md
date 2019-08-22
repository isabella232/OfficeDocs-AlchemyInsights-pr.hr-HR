---
title: Identificiranje IP adresu i klijent zapisnika nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539021"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificiranje IP adresu i klijent zapisnika nadzora

IP adresa koja odgovara aktivnost korisnika Office 365 ili administrator je prikazan u zapisnike nadzora. Klijent informacije također prijavljeni. Ovdje su koraci za označavanje takve informacije

1. Prijavite se u sustav [Office 365 sigurnosne & usklađenosti centar](https://protection.office.com/).

2. Idi na **pretraživanje** > stranicu za**pretraživanje zapisnika nadzora** .

   Ako vas zanima određenih aktivnosti, odaberite ga s popisa **aktivnosti** . Ako nije, sve aktivnosti će biti vraćene za odabranog korisnika (Zadana postavka).

   **Napomena**: određene aktivnosti možda neće biti dostupne u izborniku **aktivnosti** ; Međutim, one stavke nadzora će se vratiti ako je **Pokaži rezultate za sve aktivnosti** odabrane (Zadana postavka).

3. Navedite korisničko ime u polju **korisnicima** , odaberite odgovarajući datum raspon za aktivnost, a zatim **pretraživanje**.

U rezultatima pogledajte IP adresu za tu aktivnost u oknu rezultata. Odaberite zapis nadzora da biste vidjeli detaljne informacije Potpaleta **detalje** (na primjer, klijent, korisnik izvršiti akciju, itd.).

Dodatne informacije potražite u [pronalaženju IP adresu računala koristiti za pristup compromised računa](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
