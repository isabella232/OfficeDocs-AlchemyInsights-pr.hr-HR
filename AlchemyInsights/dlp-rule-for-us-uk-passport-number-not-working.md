---
title: DLP pravilo za SAD / UK Passport Number ne radi
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
ms.openlocfilehash: 9d9615eccd1e245bf4ca32742bfc64321dd7a8cf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714978"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemi s DLP - US / UK brojeve putovnica

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP pitanja s američkim / UK brojevima putovnica**

Imate li problema s **a Data Loss Prevention (DLP)** ne radi za sadržaj koji sadrži broj **putovnice SAD-a/UK** kada koristite dlp osjetljivu vrstu informacija u sustavu O365? Ako je tako, provjerite sadrži li vaš sadržaj potrebne informacije za ono što DLP pravila traže prilikom procjene.
  
Na primjer, za pravilo **broja broja putovnica SAD-a/Ujedinjene Kraljevine** konfigurirane s razinom pouzdanosti od 75 %, ocjenjuju se sljedeće i moraju se otkriti kako bi se pravilo pokrenulo
  
- **[Oblik zapisa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devet znamenki

- **[Uzorak:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devet uzastopnih znamenki

- **[Kontrolni zbroj:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nema šah-suma.

- **[Definicija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika je 75% uvjeren da je otkrio ovu vrstu osjetljivih informacija ako, u blizini 300 znakova:

  - Funkcija Func_usa_uk_passport pronalazi sadržaj koji odgovara uzorku.

  - Ključna riječ iz Keyword_passport je pronađena.

    Na primjer, sljedeći uzorak aktivirao bi se za pravilnik o **broju putovnica SAD-a i Ujedinjene Kraljevine:** Broj putovnice SAD-a 123456789

Dodatne informacije o tome što je potrebno za otkrivenje broja putovnice u SAD-u/UK za vaš sadržaj potražite u sljedećem odjeljku: [Što vrste osjetljivih informacija traže broj putovnice u SAD-u/Uk-u](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Pomoću druge ugrađene osjetljive vrste informacija potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: [Što zahtijevaju osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  