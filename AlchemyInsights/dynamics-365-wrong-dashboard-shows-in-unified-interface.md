---
title: Dynamics 365 - pogrešan nadzorne ploče prikazuje u sučelju Objedinjena Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747149"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Prikazuje pogrešne nadzorne ploče u sučelju Objedinjena Dynamics 365

Postoji nekoliko razloga zašto možda vidjeti drugu tablu od očekujete:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Korisnik je postaviti zadane nadzorne ploče korisnika 

Obično možete identificirati korisnika zadanu nadzornu ploču postavite ako **Postavite kao zadani** gumb Pokaži u naredbenoj traci nadzorne ploče. Podrazumevanu kontrolnu tablu korisnika nadjačat će sve druge zadane nadzorne ploče, čak i ako se zadane nadzorne ploče korisnika nije u trenutnom app.

Koristite sljedeće zaobilazno rješenje za unset njihove zadane nadzorne ploče.

1. Stvori novu nadzornu osobne.

2. Tu novu nadzornu ploču postavite kao zadani korisnik.

3. Izbrišite tu nadzornu ploču.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Nadzornu ploču postavite u na mapu lokacije

Možda ste postavili organizacije zadane nadzorne ploče odabirom nadzorne ploče i odabirom 'Postavi kao zadano' pod 'Prilagoditi sustav'. Ali nadzorne ploče definirane u dizajneru karte web-mjesta će prednost nad nadzorna ploča, ako korisnik ima pristup.

Da bi korisnici vidjeli nadzornu ploču postavite kao zadanu organizaciji, možete je:

* Postavite tu nadzornu ploču na mapu lokacije

* Uklanjanje pristupa nadzorne ploče karte definiran za one korisnike
