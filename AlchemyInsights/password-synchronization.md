---
title: Sinkronizacija lozinki
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960827"
---
# <a name="password-synchronization"></a>Sinkronizacija lozinki

**Sinkronizacija s hashom lozinke uopće ne funkcionira**

Neki uobičajeni problemi na koje korisnici naiđu kada sinkronizacija s hashom lozinke ne funkcionira:

- Računu servisa Active Directory koji koristi Azure AD Povezivanje za komunikaciju  s lokalnim servisom Active Directory ne daje se replicirati promjene direktorija i **replicirati** promjene direktorija Sve dozvole potrebne za sinkronizaciju lozinke – to morate riješiti tako da te dozvole dodijelite računu servisa Active Directory.
- Sinkronizacija hasha lozinke onemogućena je nakon što  je administrator promijenio način korisničkog Sign-In-a iz sinkronizacije lozinke na drugu mogućnost, kao što je Vanjski pristup s **AD FS-om** u čarobnjaku za Azure AD Povezivanje – to možete riješiti tako da ponovno omogućite značajku sinkronizacije **hasha** lozinke u čarobnjaku za azure AD Povezivanje.
- Problem s povezivanjem s lokalnim servisom Active Directory. Nekim kontrolerima domena, primjerice, Azure AD Povezivanje ne [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) može pristupiti ili vatrozid blokira potrebne priključke – to morate riješiti tako da se osigura pravilno povezivanje između poslužitelja azure AD Povezivanje i lokalnog servisa Active Directory.
- Poslužitelj servisa Azure AD Povezivanje trenutno je u načinu rada za postavljanje, što će uzrokovati da poslužitelj ne može koristiti hashove za lozinke – Da biste otklonili poteškoće, slijedite korake opisane u odjeljku Otklanjanje poteškoća sa sinkronizacijom lozinke sa sinkronizacijom servisa Azure AD Povezivanje – ne sinkroniziraju [se lozinke](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Sinkronizacija s hashom lozinke ne funkcionira za neke od mojih korisnika**

1. Ako ste primijetili da se hash lozinke  ne sinkronizira za korisnika, upotrijebite zadatak za otklanjanje poteškoća u servisu Azure AD Povezivanje biste istražili i riješili problem. Izvođenje sljedećih zadataka:

    a. [Pokretanje zadatka otklanjanja poteškoća u čarobnjaku](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Korištenje cmdleta za otklanjanje poteškoća radi istraživanja problema sa sinkronizacijom hasha lozinke za određenu upotrebu](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Lokalni korisnički objekt servisa Active Directory omogućen je za korisnik mora promijeniti **lozinku prilikom sljedeće mogućnosti prijave.** Kada je ta mogućnost omogućena, korisniku će se dodijeliti privremena lozinka i od vas će se zatražiti da promijeni lozinku prilikom sljedeće prijave. Azure AD Povezivanje ne sinkronizira privremene lozinke sa servisom Azure AD.

Da biste riješili gore navedeni problem, izvršite jedan od sljedećih zadataka:

- Zatražite od korisnika da se prijavi u lokalnu aplikaciju (npr. Windows desktop) i promijeni lozinku. Nova će se lozinka sinkronizirati sa servisom Azure AD.
- Neka administrator ažurira korisničku lozinku bez omogućivanja mogućnosti Korisnik mora promijeniti lozinku prilikom sljedeće prijave **i** zajednički koristiti novu lozinku s korisnikom.

3. Lokalni korisnički objekt servisa Active Directory nije pravilno **konfiguriran za sinkronizaciju objekta** ili sinkronizaciju lozinke. Da biste otklonili taj problem, slijedite korake opisane u članku Otklanjanje poteškoća sa [sinkronizacijom hasha lozinke sa servisom Azure AD Povezivanje sinkronizacijom](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







