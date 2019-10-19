---
title: Dynamics 365-pogrešna nadzorna ploča prikazuje u sustavu Dynamics 365 objedinjeno sučelje
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528543"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Pogrešna nadzorna ploča prikazuje se u sustavu Dynamics 365 objedinjeno sučelje

Postoji nekoliko razloga zašto biste mogli vidjeti drugačiju nadzornu ploču od one koju očekujete:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Korisnik je postavio zadanu nadzornu ploču korisnika 

Obično možete identificirati zadanu korisničku nadzornu ploču ako se **skup kao zadani** gumb ne pojavi na naredbenoj traci nadzorne ploče. Zadana nadzorna ploča korisnika nadjačat će sve ostale zadane nadzorne ploče, čak i ako korisnikova zadana nadzorna ploča nije u trenutnoj aplikaciji.

Za poništavanje postavljanja zadane nadzorne ploče koristite sljedeće zaobilazno rješenje.

1. Stvorite novu osobnu nadzornu ploču.

2. Postavite tu novu nadzornu ploču kao zadani korisnik.

3. Izbriši tu nadzornu ploču.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Nadzorna ploča postavljena je na karti web-mjesta

Možda ste postavili zadanu nadzornu ploču organizacije odabirom nadzorne ploče i odabirom opcije "Postavi kao zadano" pod "Prilagodi sustav". No, nadzorna ploča definirana u dizajneru web-mjesta imat će prednost nad ovom nadzornom pločom ako korisnik ima pristup njemu.

Da bi korisnici vidjeli nadzornu ploču koju ste postavili kao zadanu organizaciju, možete:

* Postavite tu nadzornu ploču na web-mjestu

* Uklanjanje pristupa definiranoj nadzornoj ploči web-mjesta za te korisnike
