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
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507398"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemi s brojevima kreditnih kartica

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s brojevima kreditnih kartica**

Imate li problema s **sprječavanjem gubitka podataka (DLP)** koji ne radi za sadržaj koji sadrži **broj kreditne kartice** kada koristite DLP osjetljivu vrstu informacija u sustavu O365? Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije da biste pokrenuli pravilo DLP-a prilikom procjene. Na primjer, da bi **pravila kreditne kartice** konfigurirana s razinom pouzdanosti od 85%, ocjenjuju se sljedeće i moraju se otkriti da bi se pravilo pokrenulo:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 znamenki koje se mogu formatirati ili neformatirane (dddddddddddddd) i moraju proći Test Luhn.

- **[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Vrlo složen i robustan uzorak koji otkriva kartice svih glavnih marki širom svijeta, uključujući Visa, MasterCard, Discover Card, JCB, American Express, poklon kartice i diner kartice.

- **[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, Luhn checksum.

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP politika je 85% sigurni da je otkrivena ova vrsta osjetljivih informacija ako, u blizini od 300 znakova:

  - Funkcija Func_credit_card pronalazi sadržaj koji odgovara uzorku.

  - Jedno od sljedećeg je istina:

  - Ključna riječ iz Keyword_cc_verification.

  - Ključna riječ Keyword_cc_name

  - Funkcija Func_expiration_date pronalazi datum u ispravnom obliku datuma.

  - Kontrolni zbroj prolazi

    Na primjer, sljedeći uzorak će se pokrenuti za DLP pravila broja kreditne kartice:

  - Visa: 4485 3647 3952 7352
  
  - Ističe: 2/2009

Dodatne informacije o tome što je potrebno za otkriven broj **kreditne kartice** za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže kreditnu karticu#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Pomoću druge ugrađene vrste osjetljivih informacija pogledajte sljedeći članak za informacije o tome što je potrebno za druge vrste: [Što traže vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  