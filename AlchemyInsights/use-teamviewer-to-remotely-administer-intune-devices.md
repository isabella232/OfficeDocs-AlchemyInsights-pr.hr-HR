---
title: Korištenje programa TeamViewer za daljinsko administriranje intune uređaja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554774"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Korištenje programa TeamViewer za daljinsko administriranje intune uređaja

Uređaji kojima upravlja Intune mogu se daljinski upravljati pomoću [programa TeamViewer](https://www.teamviewer.com/).

Da biste upravljali intune pomoću programa TeamViewer, slijedite ove korake: 

Započnite dohvaćanjem vjerodajnica od programa TeamViewer da biste postavili TeamViewer Connector na intune. To administratoru omogućuje unos vjerodajnica u korisničko ime programa TeamViewer Connector u odjeljku Uređaji, jednokratna operacija za uspostavljanje veze između servisa Intune i usluge TeamViewer.

**1. dio: pokretanje sesije pomoću udaljenog uređaja**

1. U odjeljku **Svi uređaji**odaberite uređaj s kojim želite pokrenuti udaljenu sesiju.
2. Od **... Dodatne**postavke odaberite **Nova sesija daljinske pomoći**.
3. Odaberite **Da** da biste potvrdili da želite uspostaviti udaljenu sesiju.
    Nakon što servis TeamViewer potvrdi zahtjev "Pokretanje nove udaljene sesije", vidjet ćete mogućnost **pokretanja daljinske pomoći** pod detaljima okna Pregled (ili Essentials) za uređaj. Odaberite **Vidi više** da biste proširili okno i prikazali status daljinske pomoći.
4. Odaberite **Pokreni udaljenu sesiju** da biste pokrenuli sesiju na strani administratora.
5. Odaberite preuzimanje binarnog programa TeamViewer (Windows), a zatim odaberite **Pokreni**.<br/>
    **Napomena:** Možete zanemariti bilo koju stranicu web-preglednika otvorenu na web-mjestu Programa TeamViewer.

6. Potvrdite zahtjev za aplikaciju TeamViewer da biste unijeli promjene na uređaju (samo Windows).
7. Pokreće se aplikacija TeamViewer i uključuje kôd sesije za provjeru autentičnosti veze s udaljenim uređajem.

**Dio 2: Na uređaju koji se cilja za udaljenu sesiju**

1. Otvorite portal tvrtke Intune.
2. Potražite zastavicu obavijesti: "Vaš IT administrator traži kontrolu nad ovim uređajem za sesiju daljinske pomoći" i odaberite obavijest.
3. Odaberite preuzimanje aplikacije TeamViewer ili potvrdite preuzimanje aplikacije TeamViewer iz trgovine aplikacija i odaberite **Pokreni**.
    **Napomena:** Možete zanemariti bilo koju stranicu web-preglednika otvorenu na web-mjestu Programa TeamViewer.

4. Potvrdite zahtjev za aplikaciju TeamViewer da biste unijeli promjene na uređaju (samo Windows).
5. Pokreće se aplikacija TeamViewer i uključuje kôd sesije za provjeru autentičnosti veze s udaljenim uređajem.
6. Skočni prozor pita želite li dopustiti pokretanje sesije.

**Napomena:** Šifre sesija koje generira usluga TeamViewer jednokratno su upotreba. Ako izgubite vezu, morate:

1. Zatvorite instancu aplikacije TeamViewer na udaljenom uređaju i na upravljačkoj radnoj stanici.
2. Zatvorite portal tvrtke na udaljenom uređaju.
3. Pokrenite novu "Novu sesiju daljinske pomoći" s portala za administratore.
4. Ponovno otvorite portal tvrtke na udaljenom uređaju da biste primili novu obavijest.
5. Preuzmite i otvorite aplikaciju TeamViewer na udaljenom uređaju i na administratorsku radnu stanicu, kao i prije.