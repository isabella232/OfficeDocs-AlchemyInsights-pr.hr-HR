---
title: DLP Pravilo za broj kreditne kartice ne funkcionira
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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005082"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemi s brojevima kreditnih kartica

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s brojevima kreditnih kartica**

Imate li problema s sprječavanjem gubitka podataka **(DLP)** koji ne funkcionira za sadržaj koji sadrži broj kreditne kartice prilikom korištenja vrste podataka osjetljive na DLP u sustavu O365?  Ako je tako, provjerite sadrži li sadržaj potrebne informacije za pokretanje pravilnika o DLP-u prilikom procjene. Na primjer, za pravilnik **o** kreditnoj kartici konfiguriran s razinom pouzdanosti od 85 %, procjenjuje se sljedeće i mora se otkriti da bi se pravilo pokrenulo:
  
- **[Oblik:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 znamenki koje je moguće oblikovati ili neoblikovati (dddddddddddddddddd) i moraju proći luhn test.

- **[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Vrlo složen i robusan uzorak koji otkriva kartice svih glavnih brendova diljem svijeta, uključujući Visa, MasterCard, Discover Card, JCB, American Express, poklon-bonove i kartice za restorane.

- **[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, luhn checksum

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP pravilnik 85 % je siguran da je otkrio tu vrstu osjetljivih podataka ako je u blizini 300 znakova:

  - Funkcija Func_credit_card pronalazi sadržaj koji odgovara uzorku.

  - Vrijedi nešto od sljedećeg:

  - Ključna riječ iz Keyword_cc_verification nalazi se.

  - Ključna riječ iz Keyword_cc_name nalazi se

  - Funkcija Func_expiration_date datum u desnom obliku datuma.

  - Kontrolni zbroj prolazi

    Sljedeći primjer, primjerice, aktivirao bi se za pravilnik o broju kreditne kartice za DLP:

  - Viza: 4485 3647 3952 7352
  
  - Ističe: 2.2.2009.

Dodatne informacije o tome što  je potrebno da bi se broj kreditne kartice mogao otkriti za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: Što vrste osjetljivih informacija [potražite na kreditnoj kartici#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Korištenje druge ugrađene osjetljive vrste podataka potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: Što vrste [osjetljivih informacija potražite](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  