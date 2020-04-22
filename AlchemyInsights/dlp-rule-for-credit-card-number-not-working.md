---
title: DLP pravilo za broj kreditne kartice ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704193"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemi s brojevima kreditnih kartica

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s brojevima kreditnih kartica**

Imate li problema s **sprječavanjem gubitka podataka (DLP)** koji ne radi za sadržaj koji sadrži **broj kreditne kartice** kada koristite vrstu podataka osjetljivih na DLP u sustavu O365? Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije za pokretanje pravila DLP-a prilikom procjene. Na primjer, za **pravila kreditne kartice** konfigurirane s razinom pouzdanosti od 85%, vrednuju se sljedeće i mora se otkriti da bi se pravilo pokrenulo:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 znamenki koje se mogu formatirati ili neformatirati (ddddddddddddddd) i moraju proći Luhn test.

- **[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Vrlo složen i robustan uzorak koji otkriva kartice iz svih glavnih marki širom svijeta, uključujući Visa, MasterCard, Discover Card, JCB, American Express, poklon kartice, i diner kartice.

- **[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Da, Luhn kontrolni zbroj.

- **[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politika je 85% uvjeren da je otkrio ovu vrstu osjetljivih informacija ako, u blizini 300 znakova:

  - Funkcija Func_credit_card pronalazi sadržaj koji odgovara uzorku.

  - Točno je jedno od sljedećeg:

  - Ključna riječ iz Keyword_cc_verification je pronađena.

  - Ključna riječ iz Keyword_cc_name je pronađena

  - Funkcija Func_expiration_date pronalazi datum u pravom obliku datuma.

  - Kontrolni zbroj prolazi

    Na primjer, sljedeći uzorak će se pokrenuti za DLP Credit Card Number Policy:

  - Visa: 4485 3647 3952 7352
  
  - Ističe: 2/2009

Dodatne informacije o tome što je potrebno za detektiranje **broja kreditne kartice** za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže kreditnu karticu#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Pomoću druge ugrađene osjetljive vrste informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [Što zahtijevaju osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  