---
title: Zaglavljeni u izlaznim kutijama zbog velikih privitaka
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441298"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Ispravljanje poruka koje su zaglavljeno u izlazno polje

Preporučujemo da počnete pokretanjem scenarija ["Imam problema s slanjem, primanjem ili pronalaženjem poruka e-pošte"](https://aka.ms/SaRA-OutlookSendReceive) iz alata [Microsoftova pomoćnika za podršku i oporavak](https://diagnostics.office.com/#/) .

Kada se poruka zaglavi u izlaznim sanducima, najvjerojatniji uzroci su:
- Veliki privici.
- **Pošalji odmah kada je povezana** opcija nije omogućena.

Da biste uklonili velike privitke: 

1. U programu Outlook odaberite **slanje/primanje** > **radi izvanmrežno**. 
2. U navigacijskom oknu odaberite **izlazno polje**. Odavde možete: 
    - Izbrišite poruku (odaberite je, a zatim odaberite **Izbriši**).
    - Povucite poruku u mapu Skice, dvokliknite da biste je otvorili i uklonite privitak, odaberite ga, a zatim odaberite **Izbriši**).
3. Ako primite pogrešku koja kaže da Outlook pokušava prenijeti poruku, zatvorite Outlook. Možda će trebati nekoliko trenutaka da izađete. Ako se Outlook ne zatvara, pritisnite CTRL + ALT + DELETE i odaberite **Pokreni upravitelj zadataka**. U upravitelju zadataka odaberite karticu **procesi** , pomaknite se prema dolje u Outlook. exe i odaberite **završetak procesa**.
4. Nakon što se Outlook zatvori, ponovno ga pokrenite i ponovite korake 2 i 3. 
5. Nakon što uklonite privitak, pritisnite **Pošalji/primi** > **Izvanmrežni rad** da biste nastavili raditi na mreži. 

Poruke se također zaglave u izlaznu kutiju kada kliknete **Pošalji**, ali niste povezani. Kliknite **Pošalji/primi** i pogledajte gumb **Izvanmrežni rad** . Ako je plavo, isključen si. Odaberite ga za povezivanje (gumb postaje bijel) i kliknite **Pošalji sve**.
 
Da biste omogućili **Slanje odmah kada ste povezani**:
 
- Odaberite **** > **** mogućnosti >  datoteke**napredne**.
U sekciji **Slanje i primanje** odaberite **Pošalji odmah kada je spojen**, a zatim odaberite **u redu**.
 
Za sve detalje pogledajte:
- [Videozapis: slanje ili brisanje zaglavljeno e-pošte](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-pošta ostaje u mapi Outbox dok ručno ne pokrenete operaciju slanja/primanja u programu Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
