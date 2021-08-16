---
title: Dynamics 365 – pogrešna nadzorna ploča prikazuje se u objedinjenom sučelju sustava Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101474"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Pogrešna nadzorna ploča prikazuje se u objedinjenom sučelju sustava Dynamics 365

Nekoliko je razloga zbog kojih se nadzorna ploča razlikuje od nadzorne ploče koju očekujete:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Korisnik je postavio korisničku zadanu nadzornu ploču 

Korisnička zadana nadzorna ploča obično se postavlja ako se gumb **Postavi kao zadano** ne prikazuje na naredbenoj traci nadzorne ploče. Zadana nadzorna ploča korisnika nadjačat će sve ostale zadane nadzorne ploče, čak i ako korisnikova zadana nadzorna ploča nije u trenutnoj aplikaciji.

Pomoću sljedećeg zaobilaznog rješenja otklanjajte zadane nadzorne ploče.

1. Stvorite novu osobnu nadzornu ploču.

2. Postavite novu nadzornu ploču kao korisničku zadanu.

3. Izbrišite tu nadzornu ploču.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Nadzorna ploča postavljena je u karta web-mjesta

Možda ste postavili zadanu nadzornu ploču tvrtke ili ustanove tako da odaberete nadzornu ploču i odaberete "Postavi kao zadano" u odjeljku "Prilagodba sustava". No nadzorna ploča definirana u dizajneru karte web-mjesta ima prednost nad ovom nadzornom pločom ako mu korisnik ima pristup.

Da bi korisnici vidjeli nadzornu ploču koju ste postavili kao zadanu za organizaciju, možete učiniti sljedeće:

* Postavljanje nadzorne ploče u kartama web-mjesta

* Uklanjanje pristupa definiranoj nadzornoj ploči s mapama web-mjesta za te korisnike
