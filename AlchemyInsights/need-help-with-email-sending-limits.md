---
title: Potrebna vam je pomoć s ograničenjima slanja e-pošte?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836271"
---
# <a name="need-help-with-email-sending-limits"></a>Potrebna vam je pomoć s ograničenjima slanja e-pošte?

U nastavku se primjenjuju ograničenja slanja po **dizajnu** u servisu. Dodatne informacije o tim ograničenjima dokumentirane su [ovdje](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).

- Da bismo obeshrabrili isporuku neželjenih masovnih poruka, primjenjujemo ograničenja stopa primatelja po korisniku na **sve odlazne i interne poruke.** U svim SKU-ima to ograničenje **iznosi 10 000 primatelja dnevno.**  Korisnici koji moraju poslati legitimnu masovnu komercijalnu e-poštu (npr. biltene klijenata) trebali bi koristiti davatelje usluga drugih proizvođača koji su specijalizirani za te usluge.
    - **Napomena:** kada se dosegne ograničenje broja primatelja, poruke se ne mogu slati iz poštanskog sandučića dok broj primatelja koji su poslane poruke u protekla 24 sata ne padne ispod ograničenja. Korisnik neće moći slati poruke do te točke.
- Ograničenje brzine poruke **od 30 poruka po minuti primjenjuje se** na sve SKU-ove. Time se određuje koliko poruka korisnik može poslati s računa za Exchange Online u određenom razdoblju.
- Maksimalan broj primatelja dopuštenih u poljima **Prima, Kopija** i Skrivena kopija za jednu poruku e-pošte u svim SKU-ima **jest 1000 primatelja.** Da biste prilagodili to ograničenje, [idite ovdje](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).
