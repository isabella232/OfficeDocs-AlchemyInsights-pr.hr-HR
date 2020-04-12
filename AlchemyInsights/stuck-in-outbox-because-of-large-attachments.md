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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232622"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Ispravljanje poruka koje su zaglavljene u izlaznoj pošti

Preporučujemo da pokrenete scenarij ["Imam problema sa slanjem, primanjem ili pronalaženjem poruka e-pošte"](https://aka.ms/SaRA-OutlookSendReceive) iz alata [Microsoftovpomoćnik za podršku i oporavak](https://diagnostics.office.com/#/) na zahvaćenom računalu.

Kada se poruka zaglavi u izlaznoj pošti, najvjerojatniji uzrok je veliki privitak ili opcija "Pošalji odmah kada je povezan" nije omogućena.

**Uklanjanje velikog privitka**

1. Kliknite **Slanje / primanje** > **posla izvanmrežno**. 
2. U navigacijskom oknu kliknite **Izlazna pošta**. Odavde možete: 
    - Izbrišite poruku. Samo ga odaberite i kliknite **Izbriši**.
    - Povucite poruku u **mapu skica,** dvokliknite da biste otvorili poruku i izbrišite privitak (kliknite ga i kliknite **Izbriši).**
3. Ako vam pogreška kaže da Outlook pokušava prenijeti poruku, zatvorite Outlook. Možda će trebati nekoliko trenutaka da izađete. Ako se Outlook ne zatvori, pritisnite **Ctrl+Alt+Delete,** a zatim kliknite **Pokreni upravitelj zadataka**. U upravitelju zadataka odaberite karticu **Procesi,** pomaknite se prema dolje do datoteke outlook.exe, a zatim kliknite **Završi proces**.
4. Nakon zatvaranja programa Outlook ponovno pokrenite Outlook i ponovite korake 2-3. 
5. Nakon što uklonite privitak, kliknite **Pošalji / primi** > **posao izvanmrežno** da biste poništili odabir gumba i nastavili raditi na mreži. 

Poruke se zaglave i u izlaznoj pošti kada kliknete **Pošalji**, ali niste povezani. Kliknite **Slanje/primanje** i pogledajte gumb **Izvanmrežni rad.** Ako je plava, isključen si. Kliknite ga da biste se povezali (gumb pobijeli) i kliknite **Pošalji sve**.
 
**Omogući slanje odmah nakon povezivanja**
 
1. Na kartici Datoteka kliknite **Mogućnosti**.

2. U dijaloškom okviru Mogućnosti programa Outlook kliknite **Dodatno**.

3. U odjeljku Slanje i primanje kliknite da biste omogućili **slanje odmah nakon povezivanja**. Kliknite **U redu**.
 
Za sve pojedinosti pogledajte:
- [Videozapis: Slanje ili brisanje zaglavljene e-pošte](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-pošta ostaje u mapi Izlazna pošta dok ručno ne pokrenete operaciju slanja / primanja u programu Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
