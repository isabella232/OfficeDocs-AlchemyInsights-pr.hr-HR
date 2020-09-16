---
title: Postavke pokretanja u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751127"
---
# <a name="startup-settings-in-windows-10"></a>Postavke pokretanja u sustavu Windows 10

**Promjena aplikacija koje se automatski pokreću prilikom pokretanja**

1. Idite na [postavke > aplikacije > Startup](ms-settings:startupapps?activationSource=GetHelp).

2. Provjerite je **li uključena bilo**koja aplikacija koju želite pokrenuti pri pokretanju.

**Dodavanje aplikacije koja će se automatski pokretati prilikom pokretanja**

1. Kliknite ili dodirnite **Start** , a zatim pronađite aplikaciju koju želite pokrenuti prilikom pokretanja.

2. Desnom tipkom miša kliknite aplikaciju, kliknite **više**, a zatim **Otvori mjesto datoteke**. Time se otvara mjesto na kojem se sprema prečac do aplikacije. Ako ne postoji mogućnost otvaranja lokacije datoteke, to znači da se aplikacija ne može pokrenuti prilikom pokretanja.

3. Ako je mjesto datoteke otvoreno, pritisnite **tipku s logotipom sustava Windows + R**, upišite **Shell: Startup**( **u redu**). Time se otvara mapa Startup (Polazno).

4. Kopirajte i zalijepite prečac do aplikacije s mjesta datoteke u mapu Startup (Polazno).

**Napredne mogućnosti pokretanja (uključujući siguran način rada, postavke UEFI-a i dizanje s drugog uređaja)**

1. Spremite svoj rad i Zatvori sve otvorene dokumente jer će ti koraci ponovno pokrenuti PC.

2. Idite na [postavke > ažuriranje & sigurnosnog > oporavka](ms-settings:recovery?activationSource=GetHelp).

3. U odjeljku **Napredno pokretanje**kliknite **Ponovno pokreni sada**. 

4. Kada se PC ponovno pokrene, odaberite zaslon mogućnosti:

    - Da biste se pokrenuti s uređaja kao što je USB pogon, kliknite **koristi uređaj**.

    - Da biste unijeli postavke UEFI-a (ponekad se naziva Postavljanje BIOS-a), kliknite **Otklanjanje poteškoća > dodatnim mogućnostima > postavke firmware**-a. 

    - Da biste unijeli siguran način rada ili promijenili napredne postavke pokretanja, kliknite **Otklanjanje poteškoća > dodatnim mogućnostima > postavke pokretanja**, a zatim **Ponovno pokreni**. Možda će se od vas zatražiti da unesete [BitLocker ključ oporavka](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Nakon ponovnog pokretanja PC-ja kliknite postavku pokretanja koju želite koristiti.