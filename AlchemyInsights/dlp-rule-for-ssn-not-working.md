---
title: DLP pravilo za SSN ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507362"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemi s brojevima socijalnog osiguranja

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi sa SSNs**

Imate li problema s **sprječavanjem gubitka podataka (DLP)** koji ne radi za sadržaj koji sadrži **broj socijalnog osiguranja (SSN)** kada koristite osjetljivu vrstu informacija u sustavu Microsoft 365? Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije o tome što koristi pravilo DLP-a. 
  
Na primjer, za pravilo SSN-a konfigurirano s razinom pouzdanosti od 85%, ocjenjuju se sljedeće i moraju se otkriti da bi se pravilo pokrenulo:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 znamenki, koje mogu biti u oblikovanom ili neoblikovanom uzorku

- **[Uzorak:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije traže SSN-ove u četiri različita uzorka:

  - Func_ssn pronalazi SSN-ove s jakim oblikovanjem prije 2011.

  - Func_unformatted_ssn pronalazi SSN-ove s jakim oblikovanjem prije 2011.

  - Func_randomized_formatted_ssn pronalazi SSN-ove nakon 2011.

  - Func_randomized_unformatted_ssn pronalazi SSN-ove nakon 2011.

- **[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, nema Kontrolnog zbroja.

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP politika je 85% sigurni da je otkrivena ova vrsta osjetljivih informacija ako, u blizini od 300 znakova:

  - [Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) pronalazi sadržaj koji odgovara uzorku.

  - Ključna riječ iz [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) Primjeri ključnih riječi uključuju: *socijalno osiguranje, socijalno osiguranje#, Soc Sec , SSN* . Na primjer, sljedeći uzorak pokrenuo bi se za pravilo DLP SSN-a: **SSN: 489-36-8350**
  
Dodatne informacije o tome što je potrebno za otkrivene SSN-ove za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže SSN-ove](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Pomoću druge ugrađene vrste osjetljivih informacija pogledajte sljedeći članak za informacije o tome što je potrebno za druge vrste: [Što traže vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  