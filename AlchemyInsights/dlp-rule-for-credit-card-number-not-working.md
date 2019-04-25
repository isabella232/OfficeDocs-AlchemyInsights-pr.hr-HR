---
title: DLP pravilo za broj kreditne kartice ne radi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404473"
---
Imate li problema s **Podataka gubitak Data Execution Prevention (DLP)** ne rade za sadržaj koji sadrži **Broj kreditne kartice** kada koristite vrstu osjetljive informacije DLP u O365? Ako je tako, provjerite je li vaš sadržaj sadrži potrebne informacije okidač na DLP pravila kada je procijeniti. Ako, na primjer, za **kreditne kartice pravila** konfiguriran s razinu pouzdanosti 85%, sljedeće vrednuju i morate otkrio za pravilo okidač: 
  
- **[Oblik:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 znamenki koje možete oblikovani ili neoblikovani (dddddddddddddddd) i mora proći Luhn test. 
    
- **[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Vrlo složene i robustan uzorak koji otkrije karte iz svih glavna gnojiva svijetu, uključujući Visa, Mastercard, otkrivanje kartica, JCB, American Express, poklon, i diner kartice. 
    
- **[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Da, Luhn kontrolni zbroj 
    
- **[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP pravila je % 85 sigurni da je otkrio ovu vrstu osjetljive informacije ako unutar blizine 300 znakova: 
    
  - Funkcija Func_credit_card pronalazi sadržaja koji odgovara uzorku.
    
  - Vrijedi nešto od sljedećeg: 
    
  - Ključne riječi iz Keyword_cc_verification nije pronađen.
    
  - Pronađen ključne riječi iz Keyword_cc_name
    
  - Funkcija Func_expiration_date pronalazi datum u obliku datuma desno.
    
  - Kontrolni zbroj prolaza
    
    Na primjer, sljedeći uzorak 'D okidač za DLP pravila broj kreditne kartice:
    
  - Visa: 4485 3647 3952 7352 
    
  - Istječe: 2/2009
    
Dodatne informacije na što je potreban **Broj kreditne kartice** otkrio za sadržaj potražite u sljedećoj sekciji ovog članka: [Što u osjetljive informacije vrste potražite kreditne kartice #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Pomoću različitih osjetljivih informacija za ugrađene vrste, pogledajte sljedeći članak informacije na što je potrebno za druge vrste: [što u osjetljive informacije vrste Potraži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

