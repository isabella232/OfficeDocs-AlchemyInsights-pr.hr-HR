---
title: Postavke pokretanja u Windows 10
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
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909818"
---
# <a name="startup-settings-in-windows-10"></a>Postavke pokretanja u Windows 10

**Promjena aplikacija koje se automatski pokreće prilikom pokretanja**

1. Idite na [Postavke > Aplikacije > Pokretanje](ms-settings:startupapps?activationSource=GetHelp).

2. Provjerite je li bilo koja aplikacija koju želite pokrenuti prilikom pokretanja **uključena**.

**Dodavanje aplikacije za automatsko pokretanje prilikom pokretanja**

1. Kliknite ili dodirnite **Start** pa pronađite aplikaciju koju želite pokrenuti prilikom pokretanja.

2. Desnom tipkom miša kliknite aplikaciju, zatim **Više**, a zatim **Otvori mjesto datoteke**. Time se otvara mjesto na koje se sprema prečac do aplikacije. Ako nema mogućnosti Za otvaranje mjesta datoteke, to znači da se aplikacija ne može pokrenuti prilikom pokretanja.

3. Kada je mjesto datoteke otvoreno, pritisnite tipku **s logotipom Windows + R**, upišite **shell:startup**, a zatim kliknite U **redu**. Time se otvara mapa Pokretanje.

4. Kopirajte i zalijepite prečac do aplikacije s mjesta datoteke u mapu Polazno.

**Napredne mogućnosti pokretanja (uključujući Sef, UEFI postavke i pokretanje s drugog uređaja)**

1. Spremite svoj rad i zatvorite sve otvorene dokumente jer će se ovim koracima ponovno pokrenuti PC.

2. Idite [na Postavke > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).

3. U **odjeljku Napredno pokretanje** kliknite Odmah ponovno **pokreni**. 

4. Kada se PC ponovno pokrene na zaslon Odabir mogućnosti:

    - Da biste se digli s uređaja kao što je USB pogon, **kliknite Koristi uređaj**.

    - Da biste unijeli UEFI postavke (ponekad se nazivaju postavljanjem **BIOS-a), kliknite Otklanjanje poteškoća > Dodatne mogućnosti > UEFI firmware Postavke**. 

    - Da biste Sef način rada ili promijenili napredne postavke pokretanja, **kliknite Otklanjanje poteškoća > Dodatne mogućnosti > Pokretanje Postavke**, a zatim Ponovno **pokreni**. Možda će se od vas tražiti da unesete [ključ za oporavak značajke BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Kada se PC ponovno pokrene, kliknite postavku pokretanja koju želite koristiti.