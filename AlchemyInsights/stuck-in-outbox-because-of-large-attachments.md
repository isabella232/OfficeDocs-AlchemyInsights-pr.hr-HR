---
title: Zaglavi u izlaznoj pošti zbog velikih privitaka
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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241244"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Ispravljanje poruka koje su zaglavljene u izlaznoj pošti

Preporučujemo da pokrenete scenarij ["Imam problema sa slanjem, primanjem ili pronalaženjem poruka e-pošte"](https://aka.ms/SaRA-OutlookSendReceive) iz alata [Microsoftovpomoćnik za podršku i oporavak.](https://diagnostics.office.com/#/)

Kada se poruka zaglavi u izlaznoj pošti, najvjerojatniji uzrok je veliki privitak ili opcija "Pošalji odmah kada je povezan" nije omogućena.

**Uklanjanje velikog privitka**

1. U programu Outlook odaberite **Slanje / primanje** > **izvanmrežnog rada**. 
2. U navigacijskom oknu odaberite **Izlazna pošta**. Odavde možete: 
    - Izbrišite poruku (odaberite je, a zatim odaberite **Izbriši**).
    - Povucite poruku u mapu Skice, dvokliknite da biste je otvorili i uklonite privitak, odaberite je, a zatim odaberite **Izbriši**).
3. Ako primite poruku koja kaže da Outlook pokušava prenijeti poruku, zatvorite Outlook. Možda će trebati nekoliko trenutaka da izađete. Ako se Outlook ne zatvori, pritisnite Ctrl+Alt+Delete i odaberite **Pokreni upravitelj zadataka**. U upravitelju zadataka odaberite karticu **Procesi,** pomaknite se prema dolje do datoteke outlook.exe i odaberite **Završi proces**.
4. Nakon zatvaranja programa Outlook ponovno ga pokrenite i ponovite korake 2 i 3. 
5. Nakon što uklonite privitak, kliknite **Pošalji / primi** > **izvanmrežni rad** da biste nastavili raditi na mreži. 

Poruke se zaglave i u izlaznoj pošti kada kliknete **Pošalji**, ali niste povezani. Kliknite **Slanje/primanje** i pogledajte gumb **Izvanmrežni rad.** Ako je plava, isključen si. Kliknite ga da biste se povezali (gumb pobijeli) i kliknite **Pošalji sve**.
 
**Omogući slanje odmah nakon povezivanja**
 
1. Na kartici Datoteka kliknite **Mogućnosti**.

2. U dijaloškom okviru Mogućnosti programa Outlook kliknite **Dodatno**.

3. U odjeljku Slanje i primanje kliknite da biste omogućili **slanje odmah nakon povezivanja**. Kliknite **U redu**.
 
Za sve pojedinosti pogledajte:
- [Videozapis: Slanje ili brisanje zaglavljene e-pošte](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-pošta ostaje u mapi Izlazna pošta dok ručno ne pokrenete operaciju slanja / primanja u programu Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
