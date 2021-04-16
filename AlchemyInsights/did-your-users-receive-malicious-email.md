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
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815238"
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
    - [blokiranje pristupa zlonamjernom URL-u pomoću](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) sigurnih veza
    - praćenje korisnika koji su klikali i pristupali zlonamjernim URL-ovima: Prikaz URL-a za [krađu identiteta i klika](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)na podatke o  &  [presudi Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - ručno [pokretanje automatizirane pretrage](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Možete i zaštititi od zlonamjernih datoteka i URL-ova slijedeći upute u aplikaciji [Zaštita od zlonamjernih URL-ova i datoteka](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).