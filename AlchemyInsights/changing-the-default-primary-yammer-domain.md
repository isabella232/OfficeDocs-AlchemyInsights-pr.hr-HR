---
title: Promjena zadane domene servisa Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991099"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Promjena zadane/primarne domene servisa Yammer

URL servisa Yammer sadrži trenutni primarni naziv domene za mrežu servisa Yammer. Naziv domene možda se neće podudarati s primarnim nazivom domene koji je postavljen u sustavu Office 365 ili servisu Azure AD. Postoje razlike u ponašanju koje se temelje na broju prilagođenih domena koje su dodane klijentu te ovisno o tome je li Yammer u podržanoj konfiguraciji (1 klijent: 1 mreža ili 1:1). Dostupna je dokumentacija o [Domenama servisa Yammer i sustavu Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).

Najčešći uzrok prikazivanja netočne domene jest postojanje više mreža servisa Yammer koje treba konsolidirati. [Konsolidiranje na jednu mrežu](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) pomoću alata za migraciju mreže važan je prvi korak. Dovršite ga prije nego što pokušate postaviti primarnu domenu.

**Bez prilagođenih domena**

Zadana domena klijenta (npr. fabrikam.onmicrosoft.com) koristit će se za nove klijente na servisu Yammer. Primarna domena bit će postavljena na yammer.com/fabrikam.onmicrosoft.com.

**Jedna prilagođena domena**

Yammer će automatski odabrati prilagođenu domenu klijenta (npr. fabrikam.com) kao primarnu domenu na servisu Yammer. Bit će postavljena na yammer.com/fabrikam.com. Promjenu će napraviti servis za sinkronizaciju domena, a do njenog stupanja na snagu može proći do 24 sata.

**Više prilagođenih domena**

Yammer može imati primarnu domenu koja se razlikuje od zadane domene klijenta. Budući da postoji više prilagođenih domena, Yammer ne pokušava pogoditi koja je dostupna domena točna. Morate otvoriti slučaj za podršku da biste zatražili da se primarni naziv domene promijeni u primarnu domenu po izboru.

**Dodatne informacije za otklanjanje poteškoća**

U nekim je slučajevima moguće da su domene premještene od jednog do drugog klijenta, a servis za sinkronizaciju domene nije se mogao uspješno dovršiti. Osim netočne primarne domene, možete imati i probleme s prijavom te druge probleme. Da biste riješili taj problem, možda ćete morati premjestiti domene na odgovarajuću mrežu uz pomoć Microsoftove podrške. Ta situacija zahtijeva izravnu pomoć i može potrajati neko vrijeme da bi se riješila, osobito ako je popis naziva domena vrlo dugačak. Otvorite slučaj za podršku da biste dobili pomoć u rješavanju te vrste problema.

Kada surađujete s agentom za podršku, agent će provjeriti jesu li domene potvrđene na klijentu pod vašom kontrolom. Možda će postaviti dodatna pitanja o domenama radi njihove potvrde ako se dodane vašem klijentu, ali ih nije potvrdio DNS. Radi bržeg postupka, provjerite je li DNS potvrdio domene.
