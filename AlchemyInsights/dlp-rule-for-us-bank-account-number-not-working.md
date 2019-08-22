---
title: DLP pravilo za nas broj bankovnog računa ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529851"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problemi s NAMA brojeve bankovnih računa

Imate li problema s **Podataka gubitak Data Execution Prevention (DLP)** ne rade za sadržaj koji sadrži **Broj bankovnog računa sad** kada koristite vrstu osjetljive informacije DLP u O365? Ako je tako, provjerite je li vaš sadržaj sadrži potrebne informacije za što je tražite pravila DLP prilikom procjene.
  
Ako, na primjer, za **Broj bankovnog računa za AMERIČKI** pravila konfiguriran s razinu pouzdanosti 85%, sljedeće vrednuju i morate otkrio za pravilo okidač:
  
- **[Obliku:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8 17 znamenki

- **[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8 17 uzastopne znamenki.

- **[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne postoji nijedan kontrolni zbroj

- **[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Pravila DLP je 75% sigurni da je otkrio ovu vrstu osjetljive informacije ako unutar blizine 300 znakova:

  - Regularni izraz Regex_usa_bank_account_number pronalazi sadržaja koji odgovara uzorku

  - Ključne riječi iz Keyword_usa_Bank_Account nije pronađen.

    Ako, na primjer, sljedeći uzorak 'D okidač za pravila **Sad broj bankovnog računa** : Provjera računa 78344011

Dodatne informacije na što je potrebno za **AMERIČKI broj bankovnog računa** za otkrio za sadržaj potražite u sljedećoj sekciji ovog članka: [Što u osjetljive informacije vrste potražite broj bankovnog računa za SAD](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Pomoću različitih osjetljivih informacija za ugrađene vrste, pogledajte sljedeći članak informacije na što je potrebno za druge vrste: [što u osjetljive informacije vrste Potraži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  