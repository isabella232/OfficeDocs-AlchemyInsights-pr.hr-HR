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
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977298"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP pitanja s brojevima socijalnog osiguranja

**Važno**: Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i onedrive ostanu vrlo dostupne – dodatne informacije [potražite u članku Prilagodbe privremenih značajki sustava SharePoint Online.](https://aka.ms/ODSPAdjustments)

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
  