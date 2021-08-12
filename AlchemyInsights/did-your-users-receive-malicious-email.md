---
title: Jesu li korisnici primili zlonamjernu e-poštu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929189"
---
# <a name="did-your-users-receive-malicious-email"></a>Jesu li korisnici primili zlonamjernu e-poštu?

- Sada možete prijaviti zlonamjernu e-poštu Microsoftu pomoću poslanih [administratora u centru za & usklađenosti](https://sip.protection.office.com/reportsubmission).

Poruke poslane u [podnescima administratora](https://sip.protection.office.com/reportsubmission) skeniraju se i sljedeći rezultati prikazani u podlošci detalja: 

- Ako je prilikom isporuke došlo do pogreške u provjeri autentičnosti e-pošte pošiljatelja.
- Informacije o učitavanjima pravilnika koje su mogle utjecati na ili nadjačati presudu poruke.
- Trenutni rezultati detonacije da biste vidjeli jesu li URL-ovi ili datoteke sadržane u poruci zlonamjerni ili ne.
- Povratne informacije od gradera

Ako je nadjačavanje pronađeno, ponovno se može dovršiti za nekoliko minuta. Ako nije bilo problema s provjerom autentičnosti e-pošte ili ako nadjačavanje nije utjecalo na isporuku, povratne informacije od gradera mogle bi potrajati i do jednog dana.

Ako se ne slažete s konačnom presudom o poruci, URL-u ili datoteci (blokirano vs. nije blokirano), ponovno pošaljite poruku nakon jednog dana radi ponovnog slanja. Velike su šanse da će se nakon slanja poruke ponovno promijeniti odluka.

U međuvremenu možete ukloniti zlonamjernu e-poštu iz korisničkih uštenih okvira slijedeći upute [u ovom članku.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)

- Korisnici s programom Microsoft Defender za Office 365 mogu:
    - Traženje [i brisanje sumnjive e-pošte pomoću eksplorera za prijetnje](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [korištenje Sef veze da biste blokirali pristup](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) zlonamjernom URL-u
    - praćenje korisnika koji su klikali i pristupali zlonamjernim URL-ovima: Prikaz URL-a za [krađu identiteta i klika](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)na podatke o  &  [presudi Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - ručno [pokretanje automatizirane pretrage](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Možete i zaštititi od zlonamjernih datoteka i URL-ova slijedeći upute u aplikaciji [Zaštita od zlonamjernih URL-ova i datoteka](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).