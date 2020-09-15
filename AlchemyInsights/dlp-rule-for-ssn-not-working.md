---
title: DLP pravilo za SSN ne funkcionira
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679361"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemi s brojevima socijalnog osiguranja

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s SSN-om**

Imate li problema s **prevencijom gubitka podataka (DLP)** ne radi za sadržaj koji sadrži **broj socijalnog osiguranja (SSN)** kada koristite vrstu osjetljive informacije u programu Microsoft 365? Ako je tako, provjerite sadrži li sadržaj potrebne informacije o tome što pravilnik programa DLP traži. 
  
Primjerice, ako je pravilo SSN konfigurirano uz razinu pouzdanosti od 85%, procjenjuje se sljedeće i mora se otkriti da bi se pravilo pokrenulo:
  
- **[Oblik:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 znamenaka, koje se mogu oblikovati u oblikovani ili neoblikovani uzorak

- **[Uzorak:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije traže SSN-ove u četiri različita uzorka:

  - Func_ssn pronalazi SSN-ove s pret2011 snažnim oblikovanjem koje su oblikovane crtice ili razmaci (DDD-DD-dddd ili DDD DD dddd)

  - Func_unformatted_ssn pronalazi SSN-ove s pret2011 jakim oblikovanjem koje su neoblikovane kao devet uzastopnih znamenki (ddddddddd)

  - Func_randomized_formatted_ssn pronalazi SSN-ove za post-2011 koje su oblikovane crtice ili razmaci (DDD-DD-dddd ili DDD DD dddd)

  - Func_randomized_unformatted_ssn pronalazi SSN-ove post-2011 koji su neoblikovani kao devet uzastopnih znamenki (ddddddddd)

- **[Potvrdni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, ne postoji checksum

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP pravilo je 85% pouzdano da je otkrivena ta vrsta osjetljivih podataka ako je u neposrednoj blizini znakova od 300:

  - [Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) pronalazi sadržaj koji odgovara uzorku.

  - Pronađena je ključna riječ iz [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Primjeri ključnih riječi obuhvaća:  *socijalna sigurnost, socijalna sigurnost #, soc sec, SSN*  . Na primjer, sljedeći će se uzorak pokrenuti za pravilnik o DLP SSN-u: **SSN: 489-36-8350**
  
Dodatne informacije o tome što je potrebno za prezentacije za SSN-ovi za sadržaj potražite u sljedećem odjeljku u ovom članku: [što vrste osjetljivih informacija traže SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) -ove
  
Korištenje različitih ugrađenih vrsta osjetljivih informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [što vrste osjetljivih podataka traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  