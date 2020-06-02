---
title: DLP pravilo za američki/britanski broj putovnice ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507290"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemi s DLP - Američki /Britanski brojevi putovnica

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s američkim /britanskim brojevima putovnica**

Imate li problema s **Sprječavanje gubitka podataka (DLP)** ne radi za sadržaj koji sadrži **američki / UK broj putovnice** kada koristite DLP osjetljive vrste informacija u O365? Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije o tome što pravila DLP-a traže kada se ocjenjuju.
  
Na primjer, za politiku **broja putovnica SAD-a/Ujedinjene Kraljevine** konfigurirana s razinom pouzdanosti od 75 %, ocjenjuju se sljedeće i moraju se otkriti kako bi pravilo pokrenulo
  
- **[Oblik:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet znamenki

- **[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet uzastopnih znamenki

- **[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nema Kontrolnog zbroja.

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP politika je 75% sigurni da je otkrivena ova vrsta osjetljivih informacija ako, u blizini od 300 znakova:

  - Funkcija Func_usa_uk_passport pronalazi sadržaj koji odgovara uzorku.

  - Ključna riječ iz Keyword_passport.

    Na primjer, sljedeći uzorak pokrenuo bi se za politiku **broja putovnice SAD-a/Ujedinjene Kraljevine:** Američki broj putovnice 123456789

Dodatne informacije o tome što je potrebno za otkriveni broj putovnice u SAD-u/UK-u za vaš sadržaj potražite u sljedećem odjeljku u ovom članku: [Što vrste osjetljivih informacija traže broj putovnice SAD-a i Velike Britanije](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Pomoću druge ugrađene vrste osjetljivih informacija pogledajte sljedeći članak za informacije o tome što je potrebno za druge vrste: [Što traže vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  