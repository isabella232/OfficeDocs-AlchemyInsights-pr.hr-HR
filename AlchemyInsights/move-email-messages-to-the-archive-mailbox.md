---
title: Premještanje poruka e-pošte arhiva poštanskog sandučića
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28280727"
---
Problematična arhiviranje stavki u arhivu poštanski sandučić. Provjerite je li obavite sljedeće korake:
  
1. Potvrdite da je **arhiviranje poštanski sandučić** je omogućeno. Ako nije, koristite korake u [ovom članku](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) da biste omogućili arhiva poštanskog sandučića. 
    
2. U centru za administraciju Exchange odaberite **Zadržavanja oznake** pod **Usklađenost upravljanja**, stvaranje **zadržavanja oznaka** s **Premještanje arhiva** akciju koja sadrži željenu **Zadržavanja dob**.
    
3. U centru za administraciju sustava Exchange odaberite **Pravila zadržavanja**, stvaranje **Pravila zadržavanja** i dodati to pravilo zadržavanja oznaka **Premjesti u arhivu** . 
    
4. [Dodjeljivanje pravila zadržavanja](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) poštanski sandučić određenog korisnika. Ista pravila primijenit će se na **primarni** i poštanski sandučić **arhiva** . 
    
Korisnikov poštanski sandučić trebala bi pravila arhiviranja za premještanje stavki poštanskog sandučića arhiva. Možda će biti potrebno da biste prisilili na upravljana mapa pomoćnika (MFA) za pokretanje i primijeniti nove postavke u korisnički poštanski sandučić. Pokrenite sljedeću naredbu tijekom [povezani EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) za pokretanje upravljanih Pomoćnik za mape za određene poštanski sandučić: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Dodatne informacije o postavljanju pravila arhiviranja potražite u odjeljku [Postavljanje arhiva i brisanje pravila za poštanske sandučiće](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

