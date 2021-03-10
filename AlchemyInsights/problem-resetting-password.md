---
title: Problem s ponovnim postavljanjem lozinke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692888"
---
# <a name="problems-resetting-password"></a>Problemi s ponovnim postavljanjem lozinke

Slijede neki od problema s kojima se možete suočiti prilikom ponovnog postavljanja lozinke i mogućih rješenja:

**Imam problem s resetiranju lozinki koje nisu obuhvaćene drugim kategorijama**

- Provjerite jeste li ovlašteni za ponovno postavljanje lozinki. Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke. Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.
- Provjerite razumijete li licencne preduvjete:
    - U vašoj tvrtki ili ustanovi mora biti dodijeljena najmanje jedna licenca
        - Samo oblak korisnici-bilo koji Office 365 (O365) Paid SKU ili Azure AD Basic
        - Cloud i/ili lokalni korisnici-Azure AD Premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure produktivnost Enterprise (SPE)
        - Dodatne informacije o zahtjevima za licenciranje potražite u članku [Licencne preduvjete za ponovno postavljanje lozinke za Azure ad samoposlužno](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Imam problema s testiranjem pravilnika za ponovno postavljanje lozinki koje sam postavio**

- Nedavno primijenjena pravila mogu potrajati nekoliko minuta da biste replicirali sve podatkovne centre i krajnje toиke. Fizička Udaljenost iz podatkovnog centra također će utjecati na brzinu primjene promjena.
- Testirajte s krajnjim korisnikom, a ne administratorom i pilotom s malim skupom korisnika. Pravila konfigurirana na portalu Azure primjenjuju se samo na krajnje korisnike, a ne za administratore. Microsoft nameće snažan zadani pravilnik o ponovnom postavljanju lozinki za bilo koju ulogu Azure administratora (primjerice: globalni administrator, administrator servisa Helpdesk, administrator lozinke itd.)
    - Saznajte više o [pravilima za administratore](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Želim implementirati izvornu lozinku, ali ne želim da moji korisnici registriraju dodatne sigurnosne informacije**

Unaprijed ispunite podatke za korisnike da ne bi morali! -Kao administrator možete postaviti svojstva telefona i e-pošte za svoje korisnike prije ponovnog postavljanja lozinke u svoju tvrtku ili ustanovu. To možete učiniti pomoću API-ja, PowerShell ili Azure AD Connect. Dodatne informacije:
- [Implementacija ponovnog postavljanja lozinke bez zahtjeva korisnika za registraciju](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Koje podatke koristi ponovno postavljanje lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Gumb za ponovno postavljanje lozinke je zasivljen**

Niste ovlašteni za ponovno postavljanje lozinki ovog korisnika. Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke. Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.

**Ne vidim oštricu za vraćanje izvorne lozinke**

Niste ovlašteni za ponovno postavljanje lozinki. Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke. Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.

**U odjeljku reset lozinke ne vidim članak o lokalnoj integraciji**

- Naziv lokalne integracije prikazuje se samo u hibridnim okruženjima, što znači da koristite lozinku nepotvrđenim da biste manipulirali lokalnim korisničkim lozinkama.
- Ovu oštricu ne vidite ako:
    - Ne koristite lozinku nepotvrđenim
    - Došlo je do problema s vašom instalacijom/povezivanjem lozinke za nepotvrđenim
    - Došlo je do problema s instalacijom/povezivanjem servisa Azure AD Connect
    - Dodatne upute za otklanjanje poteškoća s lozinkama za lozinke potražite u odjeljku [Otklanjanje poteškoća s lozinkom nepotvrđenim](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ne znam kako ponovno postaviti korisnikovu lozinku**

1. Prijavite se na portal Azure kao odgovarajući administrator.
1. Idite na sječivo korisnika i grupe, odaberite **Svi korisnici**.
1. Na popisu odaberite korisnika.
1. Za odabranog korisnika odaberite **Pregled**, a zatim na traci naredbi kliknite **ponovno Postavi lozinku**.
1. Slijedite upute na zaslonu.
    - U servisu Azure portal podržava se samo ponovno setovi za lozinku.

**Resetirao sam lozinku lokalnog korisnika na portalu za administratore sustava Office 365 ili mobilne aplikacije sustava Office 365, no korisnik se i dalje ne može prijaviti**

Na ovom portalu nije podržana lozinka writeback. Ponovno postavljanje korisničke lozinke na portalu Azure-portal.azure.com

