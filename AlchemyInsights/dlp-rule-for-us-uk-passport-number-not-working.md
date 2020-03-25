---
title: DLP pravilo za SAD / UK Passport Number ne radi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931254"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemi s DLP - US / UK brojeve putovnica

**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini. To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja. Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.

U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana. Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena. Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.

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
  