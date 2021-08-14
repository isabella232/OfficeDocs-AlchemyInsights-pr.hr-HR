---
title: DLP pravilo za američki broj bankovnog računa ne funkcionira
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
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005010"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problemi s američkim brojevima bankovnih računa

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s američkim brojevima bankovnih računa**

Imate li problema s sprječavanjem gubitka podataka **(DLP)** koji ne funkcionira za sadržaj koji sadrži američki broj bankovnog računa prilikom korištenja vrste podataka osjetljive na DLP u sustavu O365?  Ako je tako, provjerite sadrži li sadržaj potrebne informacije o tome što DLP pravilnik traži prilikom procjene.
  
Na primjer, za pravilnik **o broju bankovnog** računa u SAD-u konfiguriran s razinom pouzdanosti od 85 %, procjenjuje se sljedeće i mora se otkriti da bi se pravilo pokrenulo:
  
- **[Oblik:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** od 8 do 17 znamenki

- **[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8 do 17 uzastopnih znamenki.

- **[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nema kontrolnog zbroja

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP pravilnik je 75 % siguran da je otkrio tu vrstu osjetljivih podataka ako je u blizini 300 znakova:

  - Regularni izraz Regex_usa_bank_account_number pronalazi sadržaj koji odgovara uzorku

  - Ključna riječ iz Keyword_usa_Bank_Account nalazi se.

    Sljedeći primjer, primjerice, aktivirao bi se za pravilnik **o broju bankovnog** računa u SAD-u: provjera 78344011

Dodatne informacije o tome što  je potrebno za detektirati broj bankovnog računa u SAD-u za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: Što osjetljive vrste podataka potražite u odjeljku [Broj bankovnog računa u SAD-u](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Korištenje druge ugrađene osjetljive vrste podataka potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: Što vrste [osjetljivih informacija potražite](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  