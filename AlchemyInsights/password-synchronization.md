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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481144"
---
# <a name="password-synchronization"></a>Sinkronizacija lozinki

**Sinkronizacija zaporke za lozinke ne funkcionira uopće**

Neki Česti problemi s kojima se korisnici susreću kada sinkronizacija lozinke ne funkcionira:

- Račun za Active Directory koji koristi Azure AD Connect da bi komunicirala s lokalnim aktivnim imenikom nije odobreno **repliciranje promjena direktorija** i **Replicacijski direktorij mijenja sve** dozvole, koje su potrebne za sinkronizaciju lozinki – morate to riješiti tako da dodijelite ove dozvole za račun servisa Active Directory.
- Sinkronizacija zaporke za lozinke onemogućena je nakon što je administrator izmijenio način korištenja korisničke Sign-In iz **sinkronizacije lozinki** u neku drugu mogućnost, kao što je **Federacija sa programom AD FS** u čarobnjaku za Azure ad Connect – to možete riješiti ponovnim omogućivanjem značajke **sinkronizacije zaporke za lozinke** u čarobnjaku za Azure ad Connect.
- Problem s povezivanjem s lokalnim aktivnim imenikom. Primjerice, nekim kontrolorima domena nije moguće pristupiti pomoću servisa Azure AD Connect ili je vatrozid [potreban](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) da biste ga blokirali, morate to riješiti tako da veza između poslužitelja Azure ad Connect i lokalnog servisa Active Directory funkcionira ispravno.
- Poslužitelj za Azure AD Connect trenutno se nalazi u načinu rada za uključivanje u modu, što će prouzročiti da poslužitelj ne može otkloniti lozinku – da biste otklonili problem, slijedite korake opisane u odjeljku [Otklanjanje poteškoća s sinkronizacijom lozinke pomoću servisa Azure ad Connect sync – ne sinkroniziraju se lozinke](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Sinkronizacija lozinki za lozinke ne funkcionira za neke korisnike**

1. Ako ste primijetili da se dodatak za lozinke ne sinkronizira za korisnika, upotrijebite zadatak **otklanjanja poteškoća** u programu Azure ad Connect da biste istražili i riješili problem. Izvedite sljedeće zadatke:

    je. [Pokretanje zadatka otklanjanja poteškoća u čarobnjaku](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Korištenje cmdleta za otklanjanje poteškoća radi istraživanja problema s sinkronizacijom lozinke za određeno korištenje](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Korisnički objekt lokalnog imenika Active Directory omogućen je za **korisnika mora promijeniti lozinku pri sljedećoj mogućnosti prijave** . Kada je ta mogućnost omogućena, korisniku se dodjeljuje privremena lozinka i od vas će se zatražiti da promijenite lozinku na sljedećoj prijavi. Azure AD Connect ne sinkronizira privremene lozinke za Azure AD.

Da biste riješili gore navedeni problem, izvedite neki od sljedećih zadataka:

- Zatražite od korisnika da se prijavi u lokalnu aplikaciju (primjerice, stolna računala sa sustavom Windows) i promijenite lozinku. Nova lozinka sinkronizirat će se sa servisom Azure AD.
- Administrator će ažurirati korisničku lozinku bez omogućivanja mogućnosti da **korisnik mora promijeniti lozinku pri sljedećoj prijavi** i zajednički koristiti novu lozinku s korisnikom.

3. Lokalni objekt servisa Active Directory **nije pravilno konfiguriran** za sinkronizaciju objekata ili sinkronizaciju lozinki. Da biste riješili taj problem, slijedite korake opisane u [članku Otklanjanje poteškoća sa sinkroniziranjem lozinke uz sinkronizaciju servisa Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







