---
title: DLP pravilo za američki broj bankovnog računa ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507326"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problemi s američkim brojevima bankovnih računa

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s američkim brojevima bankovnih računa**

Imate li problema s **sprječavanjem gubitka podataka (DLP)** koji ne radi za sadržaj koji sadrži **broj bankovnog računa SAD-a** kada koristite vrstu osjetljivih informacija o DLP-u u sustavu O365? Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije o tome što pravila DLP-a traže kada se ocjenjuju.
  
Na primjer, za pravilo **broja bankovnog računa SAD-a** konfigurirano s razinom pouzdanosti od 85%, ocjenjuju se sljedeće i moraju se otkriti da bi se pravilo pokrenulo:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 znamenki

- **[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 uzastopnih znamenki.

- **[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nema Kontrolnog zbroja.

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP politika je 75% sigurni da je otkrivena ova vrsta osjetljivih informacija ako, u blizini od 300 znakova:

  - Regularni izraz Regex_usa_bank_account_number pronalazi sadržaj koji odgovara uzorku

  - Ključna riječ iz Keyword_usa_Bank_Account.

    Na primjer, sljedeći uzorak pokrenuo bi se za pravila **broja bankovnog računa SAD-a:** Tekući račun 78344011

Dodatne informacije o tome što je potrebno za **otkriveni broj bankovnog računa SAD-a** za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže broj američkog bankovnog računa](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Pomoću druge ugrađene vrste osjetljivih informacija pogledajte sljedeći članak za informacije o tome što je potrebno za druge vrste: [Što traže vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  