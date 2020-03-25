---
title: DLP pravilo za broj američkog bankovnog računa ne radi
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
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932507"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problemi s američkim brojevima bankovnih računa

**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini. To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja. Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.

U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana. Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena. Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.

**DLP problemi s američkim brojevima bankovnih računa**

Imate li problema s **a Data Loss Prevention (DLP)** ne radi za sadržaj koji sadrži broj računa **američke banke** kada koristite DLP osjetljive vrste informacija u O365? Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije za ono što DLP pravila traže prilikom procjene.
  
Na primjer, za pravilnik **o broju bankovnog računa SAD-a** konfiguriranog s razinom pouzdanosti od 85 %, vrednuju se sljedeće i mora se otkriti da bi se pravilo pokrenulo:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 znamenki

- **[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 uzastopnih znamenki.

- **[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nema šah-suma.

- **[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP politika je 75% uvjeren da je otkrio ovu vrstu osjetljivih informacija ako, u blizini 300 znakova:

  - Regularni izraz Regex_usa_bank_account_number pronalazi sadržaj koji odgovara uzorku

  - Ključna riječ iz Keyword_usa_Bank_Account je pronađena.

    Na primjer, sljedeći uzorak će se pokrenuti za **pravilnik o broju bankovnog računa SAD-a:** Tekući račun 78344011

Dodatne informacije o tome što je potrebno za detektiranje broja bankovnog računa u **SAD-u** za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže broj bankovnog računa u SAD-u](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Pomoću druge ugrađene osjetljive vrste informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [Što zahtijevaju osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  