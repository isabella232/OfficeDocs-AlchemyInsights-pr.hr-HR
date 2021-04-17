---
title: Postavke pokretanja u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828144"
---
# <a name="startup-settings-in-windows-10"></a>Postavke pokretanja u sustavu Windows 10

**Promjena aplikacija koje se automatski pokreće prilikom pokretanja**

1. Otvorite [Postavke > aplikacije > Pokretanje](ms-settings:startupapps?activationSource=GetHelp).

2. Provjerite je li bilo koja aplikacija koju želite pokrenuti prilikom pokretanja **uključena**.

**Dodavanje aplikacije za automatsko pokretanje prilikom pokretanja**

1. Kliknite ili dodirnite **Start** pa pronađite aplikaciju koju želite pokrenuti prilikom pokretanja.

2. Desnom tipkom miša kliknite aplikaciju, zatim **Više**, a zatim **Otvori mjesto datoteke**. Time se otvara mjesto na koje se sprema prečac do aplikacije. Ako nema mogućnosti Za otvaranje mjesta datoteke, to znači da se aplikacija ne može pokrenuti prilikom pokretanja.

3. Kada je mjesto datoteke otvoreno, pritisnite tipku s logotipom **sustava Windows + R**, upišite **shell:startup**, a zatim kliknite U **redu**. Time se otvara mapa Pokretanje.

4. Kopirajte i zalijepite prečac do aplikacije s mjesta datoteke u mapu Polazno.

**Napredne mogućnosti pokretanja (uključujući siguran način rada, postavke UEFI-ja i pokretanje s drugog uređaja)**

1. Spremite svoj rad i zatvorite sve otvorene dokumente jer će se ovim koracima ponovno pokrenuti PC.

2. Idite [na Postavke > Ažuriranje & sigurnost > oporavak](ms-settings:recovery?activationSource=GetHelp).

3. U **odjeljku Napredno pokretanje** kliknite Odmah ponovno **pokreni**. 

4. Kada se PC ponovno pokrene na zaslon Odabir mogućnosti:

    - Da biste se digli s uređaja kao što je USB pogon, **kliknite Koristi uređaj**.

    - Da biste unijeli UEFI postavke (ponekad se nazivaju postavljanjem **BIOS-a), kliknite Otklanjanje poteškoća > dodatne mogućnosti > postavke UEFI opreme**. 

    - Da biste unijeli sigurni način rada ili promijenili napredne postavke pokretanja, **kliknite Otklanjanje poteškoća > dodatne mogućnosti > postavke pokretanja**, a zatim ponovno **pokreni**. Možda će se od vas tražiti da unesete [ključ za oporavak značajke BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Kada se PC ponovno pokrene, kliknite postavku pokretanja koju želite koristiti.