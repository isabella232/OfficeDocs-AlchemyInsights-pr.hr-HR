---
title: DLP pravilo za SAD / velika Britanija Passport broj ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529911"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemi s DLP - sad / brojevi Passport velika Britanija

Imate problema s **Podataka gubitak Data Execution Prevention (DLP)** ne rade za sadržaja koji sadrži na **sad / velika Britanija Passport broj** prilikom korištenja vrsta osjetljive informacije DLP u O365? Ako je tako, provjerite je li vaš sadržaj sadrži potrebne informacije za što je tražite pravila DLP prilikom procjene.
  
Na primjer, za na **sad / velika Britanija Passport broj** pravila konfiguriran s razinu pouzdanosti 75% sljedeće vrednuju i morate otkrio za pravilo okidač
  
- **[Obliku:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devet znamenki

- **[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devet uzastopne znamenki

- **[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne postoji nijedan kontrolni zbroj

- **[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Pravila DLP je 75% sigurni da je otkrio ovu vrstu osjetljive informacije ako unutar blizine 300 znakova:

  - Funkcija Func_usa_uk_passport pronalazi sadržaja koji odgovara uzorku.

  - Ključne riječi iz Keyword_passport nije pronađen.

    Ako, na primjer, sljedeći uzorak bi okidač za u **sad / velika Britanija Passport broj** pravila: SAD Passport broj 123456789

Dodatne informacije na što je potrebno za u SAD / velika Britanija Passport broj otkrio za sadržaj, pogledajte sljedeći odjeljak u ovom članku: [što u osjetljive informacije vrste izgleda za SAD / velika Britanija Passport broj](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Pomoću različitih osjetljivih informacija za ugrađene vrste, pogledajte sljedeći članak informacije na što je potrebno za druge vrste: [što u osjetljive informacije vrste Potraži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  