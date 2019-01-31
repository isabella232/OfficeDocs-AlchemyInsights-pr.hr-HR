---
title: DLP pravilo za MBG ne radi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 7242bf2b101b45fec0fe00ab33fa6db150004ee5
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657351"
---
Imate li problema s **Podataka gubitak Data Execution Prevention (DLP)** za sadržaj koji sadrži **Broj socijalnog osiguranja (MBG)** kada koristite vrstu osjetljive informacije u Office 365 ne radi? Ako je tako, provjerite je li vaš sadržaj sadrži potrebne informacije za što pravila DLP izgleda. 
  
Ako, na primjer, za MBG pravila konfigurirana s razinu pouzdanosti 85%, sljedeće vrednuju i morate otkrio za pravilo okidač:
  
- **[Oblik:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 znamenki, što može biti oblikovani ili neoblikovani uzorak 
    
- **[Uzorak:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije Potraži SSNs četiri različite uzorci: 
    
  - Func_ssn pronalazi SSNs s pre 2011 Snažno oblikovanje koje su oblikovane tim crtice ili razmaka (ddd dd dddd ili ddd dd dddd)
    
  - Func_unformatted_ssn pronalazi SSNs s pre 2011 Snažno oblikovanje koje su Neoblikovani kao devet uzastopne znamenke (ddddddddd)
    
  - Func_randomized_formatted_ssn pronalazi Proknjiži 2011 SSNs koji su oblikovani crtice ili razmaka (ddd dd dddd ili ddd dd dddd)
    
  - Func_randomized_unformatted_ssn pronalazi Proknjiži 2011 SSNs koje su Neoblikovani kao devet uzastopne znamenke (ddddddddd)
    
- **[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne postoji nijedan kontrolni zbroj 
    
- **[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP pravila je % 85 sigurni da je otkrio ovu vrstu osjetljive informacije ako unutar blizine 300 znakova: 
    
  - [Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) pronalazi sadržaja koji odgovara uzorku. 
    
  - Ključne riječi iz [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) nije pronađen. Primjeri ključne riječi uključuje: *JMBG, JMBG #, PnP sek, zdravstvene Iskaznice* . Ako, na primjer, sljedeći uzorak 'D okidač MBG DLP pravila: **MBG: 489-36-8350**
    
Dodatne informacije na što je potrebno za SSNs otkrio za sadržaj potražite u sljedećoj sekciji ovog članka: [Što u osjetljive informacije vrste izgledaju SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Pomoću različitih osjetljivih informacija za ugrađene vrste, pogledajte sljedeći članak informacije na što je potrebno za druge vrste: [što u osjetljive informacije vrste Potraži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

