---
title: DLP pravilo za SSN ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932513"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP pitanja s brojevima socijalnog osiguranja

**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini. To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja. Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.

U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana. Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena. Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.

**DLP problemi sa SSN-ovima**

Imate li problema s **sprječavanjem gubitka podataka (DLP)** koji ne funkcionira za sadržaj koji sadrži **broj socijalnog osiguranja (SSN)** prilikom korištenja osjetljive vrste podataka u sustavu Office 365? Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije za ono što traži DLP pravila. 
  
Na primjer, za ssn pravilo konfigurirano s razinom pouzdanosti od 85%, vrednuju se sljedeće i mora se otkriti da bi se pravilo pokrenulo:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 znamenki, koje mogu biti u oblikovanom ili neformatiranom uzorku

- **[Uzorak:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije traže SSN-ove u četiri različita uzorka:

  - Func_ssn pronalazi SSN-ove s jakim oblikovanjem prije 2011.

  - Func_unformatted_ssn pronalazi SSN-ove s jakim oblikovanjem prije 2011.

  - Func_randomized_formatted_ssn pronalazi SSN-ove za razdoblje nakon 2011.

  - Func_randomized_unformatted_ssn pronalazi SSN-ove nakon 2011.

- **[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, nema šah-suma.

- **[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politika je 85% uvjeren da je otkrio ovu vrstu osjetljivih informacija ako, u blizini 300 znakova:

  - [Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) pronalazi sadržaj koji odgovara uzorku.

  - Ključna riječ iz [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) je pronađena. Primjeri ključnih riječi uključuju: *socijalno osiguranje, socijalno osiguranje#, Soc Sec , SSN* . Na primjer, sljedeći uzorak aktivirao bi se za politiku DLP SSN-a: **SSN: 489-36-8350**
  
Dodatne informacije o tome što je potrebno za otkrivenje SSN-ova za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Koje vrste osjetljivih informacija traže SSN-ove](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Pomoću druge ugrađene osjetljive vrste informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [Što zahtijevaju osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  