---
title: Dinamika 365 – pogrešna nadzorna ploča u sustavu Dynamics 365 Unified Interface
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
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711267"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Pogrešan prikaz nadzorne ploče u sustavu Dynamics 365 Unified Interface

Postoji nekoliko razloga zbog kojih možete vidjeti neku drugu nadzornu ploču od one koju očekujete:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Korisnik je postavio zadanu nadzornu ploču korisnika 

Obično je moguće identificirati zadanu nadzornu ploču korisnika, ako se gumb **Postavi kao zadani** ne prikazuje na naredbenom traku nadzorne ploče. Zadana nadzorna ploča korisnika nadjačat će sve druge zadane nadzorne ploče, čak i ako se zadana nadzorna ploča korisnika ne nalazi u aktualnoj aplikaciji.

Da biste poništili zadanu nadzornu ploču, upotrijebite sljedeće zaobilazno rješenje.

1. Stvorite novu osobnu nadzornu ploču.

2. Postavite tu novu nadzornu ploču kao zadanu korisniku.

3. Izbrišite tu nadzornu ploču.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Nadzorna ploča postavljena je na web-stranici Sitemap

Možda ste postavili zadanu nadzornu ploču tvrtke ili ustanove tako da odaberete nadzornu ploču i odaberete "Postavi kao zadano" u odjeljku "Prilagodba sustava". No nadzorna ploča definirana u dizajneru Sitemap imat će prednost nad tom nadzornom tabicom ako korisnik ima pristup.

Da bi korisnici mogli vidjeti nadzornu ploču koju ste postavili kao zadanu za tvrtku ili ustanovu, možete učiniti sljedeće:

* Postavljanje nadzorne ploče u mapi Sitemap

* Uklanjanje pristupa definiranoj nadzornoj ploči web-stranice za te korisnike
