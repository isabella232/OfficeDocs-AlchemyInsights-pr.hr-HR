---
title: DLP pravilo za SAD / velika Britanija Passport broj ne radi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 5722f7b6c9a2f905fed2ef4164787e020260edf7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656415"
---
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
  

