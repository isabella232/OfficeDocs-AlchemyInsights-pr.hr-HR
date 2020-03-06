---
title: Postavke pokretanja u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2020
ms.locfileid: "42408971"
---
# <a name="startup-settings-in-windows-10"></a>Postavke pokretanja u sustavu Windows 10

**Promjena aplikacija koje se automatski pokreću pri pokretanju**

1. Idite na [Postavke > aplikacije > pokretanje](ms-settings:startupapps?activationSource=GetHelp).

2. Provjerite je li uključena neka aplikacija koju želite pokrenuti pri pokretanju **.**

**Dodavanje aplikacije za automatsko pokretanje pri pokretanju**

1. Kliknite ili dodirnite **Start** i pronađite aplikaciju koju želite pokrenuti pri pokretanju.

2. Desnom tipkom miša kliknite aplikaciju, kliknite **Više**, a zatim **Otvori mjesto datoteke**. Time se otvara mjesto na koje se sprema prečac do aplikacije. Ako ne postoji mogućnost za otvaranje mjesta datoteke, to znači da se aplikacija ne može pokrenuti pri pokretanju.

3. Dok je mjesto datoteke otvoreno, pritisnite **tipku s logotipom sustava Windows + R**, upišite **shell:startup**, a zatim kliknite **U redu**. Otvorit će se mapa Startup (Pokretanje).

4. Kopirajte i zalijepite prečac do aplikacije s mjesta datoteke u mapu Pokretanje.

**Napredne mogućnosti pokretanja (uključujući siguran način rada, postavke UEFI-ja i dizanje s drugog uređaja)**

1. Spremite svoj rad i zatvorite sve otvorene dokumente jer će se ovim koracima ponovno pokrenuti PC.

2. Idite na [Postavke > Ažuriranje & sigurnosnog > Oporavak](ms-settings:recovery?activationSource=GetHelp).

3. U **odjeljku Napredno pokretanje**kliknite Odmah ponovno **pokreni**. 

4. Nakon ponovnog pokretanja PC-ja na zaslon Odabir mogućnosti:

    - Da biste se digli s uređaja kao što je USB pogon, kliknite **Koristi uređaj**.

    - Da biste unijeli postavke UEFI-ja (ponekad se nazivaju postavljanje BIOS-a), kliknite **Otklanjanje poteškoća > dodatne mogućnosti > postavkama firmvera UEFI-ja**. 

    - Da biste ušli u siguran način rada ili promijenili napredne postavke pokretanja, kliknite **Otklanjanje poteškoća > dodatne mogućnosti > postavke pokretanja,** a zatim kliknite Ponovno **pokreni**. Možda ćete morati unijeti [bitlocker ključ oporavka](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Nakon ponovnog pokretanja PC-ja kliknite postavku pokretanja koju želite koristiti.