---
title: DLP pravilo za nas/broj putovnica u Velikoj Britaniji ne funkcionira
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679216"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemi s brojem putovnica za DLP-US/UK

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s brojem putovnica za US/UK**

Imate li problema s **prevencijom gubitka podataka (DLP)** koji ne funkcionira za sadržaj koji sadrži **broj putovnice za US/UK** kada koristite DLP osjetljive informacije u programu O365? Ako je tako, provjerite sadrži li sadržaj potrebne informacije o tome što pravilnik programa DLP traži kada se procjenjuje.
  
Primjerice, za pravilnik o **broju putovnica za US/UK** konfiguriran uz razinu pouzdanosti od 75%, procjenjuje se sljedeće i mora se otkriti da bi se pravilo pokrenulo
  
- **[Oblikovanje:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet znamenki

- **[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet uzastopnih znamenki

- **[Potvrdni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ne postoji checksum

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP pravilo je 75% pouzdano da je otkrivena ta vrsta osjetljivih podataka ako je u neposrednoj blizini znakova od 300:

  - Funkcija Func_usa_uk_passport pronalazi sadržaj koji odgovara uzorku.

  - Pronađena je ključna riječ iz Keyword_passport.

    Primjerice, sljedeći će se uzorak pokrenuti za pravilnik o **broju putovnica Sjedinjenih Američkih Država/UK** : Američka putovnica broj 123456789

Dodatne informacije o tome što je potrebno za broj putovnica za US/UK da bi se otkrilo za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [što vrste osjetljivih informacija traže nas/broj putovnica Britanije](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Korištenje različitih ugrađenih vrsta osjetljivih informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [što vrste osjetljivih podataka traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  