---
title: DLP pravilo za američki/uk broj putovnice ne funkcionira
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004938"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemi s DLP-om – brojevi putovnica u SAD-u/Velikoj Britaniji

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi s američkim/britanskim brojevima putovnica**

Imate li problema s sprječavanjem gubitka podataka **(DLP)** koji ne funkcionira za sadržaj koji sadrži broj putovnice u **SAD-u/Velikoj** Britaniji prilikom korištenja vrste podataka osjetljivih na DLP u sustavu O365? Ako je tako, provjerite sadrži li sadržaj potrebne informacije o tome što DLP pravilnik traži prilikom procjene.
  
Na primjer, za pravilnik o broju putovnica u **SAD-u/Velikoj** Britaniji konfiguriran s razinom pouzdanosti od 75 %, procjenjuje se sljedeće i mora se otkriti da bi pravilo pokrenulo
  
- **[Oblikovanje:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet znamenki

- **[Uzorak:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet uzastopnih znamenki

- **[Kontrolni zbroj:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nema kontrolnog zbroja

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP pravilnik je 75 % siguran da je otkrio tu vrstu osjetljivih podataka ako je u blizini 300 znakova:

  - Funkcija Func_usa_uk_passport pronalazi sadržaj koji odgovara uzorku.

  - Ključna riječ iz Keyword_passport nalazi se.

    Na primjer, sljedeći uzorak aktivirao bi se za pravilnik o broju putovnica u **SAD-u/Ujedinjenom** Kraljevstvu: američki broj putovnice 123456789

Dodatne informacije o tome što je potrebno da bi se za vaš sadržaj otkrio broj putovnice u SAD-u/Ujedinjenom Kraljevstvu potražite u sljedećem odjeljku u ovom članku: Što osjetljive vrste podataka potražite u članku Broj putovnice [u SAD-u/Ujedinjenom Kraljevstvu](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Korištenje druge ugrađene osjetljive vrste podataka potražite u sljedećem članku informacije o tome što je potrebno za druge vrste: Što vrste [osjetljivih informacija potražite](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  