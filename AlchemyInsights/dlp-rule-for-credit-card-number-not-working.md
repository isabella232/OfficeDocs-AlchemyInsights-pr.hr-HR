---
title: DLP pravilo za broj kreditne kartice ne funkcionira
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679433"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemi s brojevima kreditnih kartica

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s brojevima kreditnih kartica**

Imate li problema s **prevencijom gubitka podataka (DLP)** ne radi za sadržaj koji sadrži **broj kreditne kartice** kada koristite DLP osjetljive informacije u O365? Ako je tako, provjerite sadrži li sadržaj potrebne informacije da biste pokrenuli pravilnik programa DLP kada se procjenjuje. Primjerice, ako je **pravilnik o kreditnoj kartici** konfiguriran s razinom pouzdanosti od 85%, procjenjuje se sljedeće i mora se otkriti da bi se pravilo pokrenulo:
  
- **[Oblik:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 znamenaka koje je moguće formatirati ili neoblikovati (dddddddddddddddde) i mora proći kroz Luhn test.

- **[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Vrlo složen i robustan uzorak koji detektira kartice svih glavnih marki diljem svijeta, uključujući vizu, MasterCard, Discover Card, JCB, American Express, poklon-bonove i kartice Diner.

- **[Potvrdni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, Luhn ček

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP pravilo je 85% pouzdano da je otkrivena ta vrsta osjetljivih podataka ako je u neposrednoj blizini znakova od 300:

  - Funkcija Func_credit_card pronalazi sadržaj koji odgovara uzorku.

  - Vrijedi jedno od sljedećeg:

  - Pronađena je ključna riječ iz Keyword_cc_verification.

  - Pronađena je ključna riječ iz Keyword_cc_name

  - Funkcija Func_expiration_date pronalazi Datum u pravom obliku datuma.

  - Potvrdni zbroj prolazi

    Na primjer, sljedeći uzorak potaknuti će pravilnik o broju kartica za DLP:

  - Viza: 4485 3647 3952 7352
  
  - Istječe: 2/2009

Dodatne informacije o potrebi otkrivanja **broja kreditnih kartica** za sadržaj potražite u sljedećem odjeljku u ovom članku: [što vrste osjetljivih informacija traže kreditnu karticu #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Korištenje različitih ugrađenih vrsta osjetljivih informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [što vrste osjetljivih podataka traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  