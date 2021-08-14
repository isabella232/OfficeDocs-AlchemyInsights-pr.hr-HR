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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004974"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemi s brojevima socijalnog osiguranja

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s SSN-om**

Imate li problema s sprječavanjem gubitka podataka **(DLP)** koji ne funkcionira za sadržaj koji sadrži broj socijalnog osiguranja **(SSN)** prilikom korištenja osjetljive vrste podataka u Microsoft 365? Ako je tako, provjerite sadrži li sadržaj potrebne informacije o tome što DLP pravilnik traži. 
  
Na primjer, za pravilnik SSN konfiguriran s razinom pouzdanosti od 85%, procjenjuje se sljedeće i mora se otkriti da bi se pravilo pokrenulo:
  
- **[Oblikovanje:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 znamenki, koje mogu biti u oblikovanom ili neoblikovljenom uzorku

- **[Uzorak:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije u četiri različita uzorka potražite SSN-ove:

  - Func_ssn pronalazi SSN-ove s jakim oblikovanjem prije 2011. oblikovanim crticama ili razmacima (ddd-dd-dddd OR ddd dddd)

  - Func_unformatted_ssn pronalazi SSN-ove s jakim oblikovanjem prije 2011. koje nije oblikovano kao devet uzastopnih znamenki (ddddddddddd)

  - Func_randomized_formatted_ssn pronalazi SSN-ove nakon 2011. oblikovane crticama ili razmacima (ddd-dd-dddd OR ddd dddd)

  - Func_randomized_unformatted_ssn pronalazi SSN-ove nakon 2011. koji nisu oblikovani kao devet uzastopnih znamenki (ddddddddddd)

- **[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, nema kontrolnog zbroja

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP pravilnik 85 % je siguran da je otkrio tu vrstu osjetljivih podataka ako je u blizini 300 znakova:

  - Funkcija [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) pronalazi sadržaj koji odgovara uzorku.

  - Ključna riječ [iz Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) nalazi se. Primjeri ključnih riječi obuhvaćaju: *socijalnu sigurnost, socijalnu sigurnost#, Soc Sec, SSN.* Sljedeći primjer, primjerice, aktivirao bi se za pravilnik DLP SSN: **SSN: 489-36-8350**
  
Dodatne informacije o tome što je potrebno za SSN-ove za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: Što vrste osjetljivih informacija [izgledaju za SSN-ove](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Korištenje druge ugrađene osjetljive vrste podataka potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: Što vrste [osjetljivih informacija potražite](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  