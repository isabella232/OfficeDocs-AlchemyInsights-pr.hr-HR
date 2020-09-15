---
title: DLP pravilo za broj bankovnog računa za US ne funkcionira
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679288"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problemi s brojevima bankovnog računa za US

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s brojevima bankovnog računa za US**

Imate li problema s **prevencijom gubitka podataka (DLP)** ne radi za sadržaj koji sadrži **broj bankovnog računa za US** kada koristite DLP osjetljivu vrstu podataka u programu O365? Ako je tako, provjerite sadrži li sadržaj potrebne informacije o tome što pravilnik programa DLP traži kada se procjenjuje.
  
Primjerice, za pravila **broja bankovnog računa za US** koja je konfigurirana uz razinu pouzdanosti od 85%, procjenjuje se sljedeće i mora se otkriti da bi se pravilo pokrenulo:
  
- **[Oblikovanje:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 znamenaka

- **[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 uzastopnih znamenki.

- **[Potvrdni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ne postoji checksum

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP pravilo je 75% pouzdano da je otkrivena ta vrsta osjetljivih podataka ako je u neposrednoj blizini znakova od 300:

  - Uobičajeni izraz Regex_usa_bank_account_number pronalazi sadržaj koji odgovara uzorku

  - Pronađena je ključna riječ iz Keyword_usa_Bank_Account.

    Na primjer, sljedeći će se uzorak pokrenuti za pravilnik o **broju bankovnog računa u sad** -u: tekući račun 78344011

Dodatne informacije o tome što je potrebno za **broj bankovnog računa za US** da bi se otkrilo za sadržaj potražite u sljedećem odjeljku u ovom članku: [što vrste osjetljivih podataka traže broj bankovnog računa za nas](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Korištenje različitih ugrađenih vrsta osjetljivih informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [što vrste osjetljivih podataka traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  