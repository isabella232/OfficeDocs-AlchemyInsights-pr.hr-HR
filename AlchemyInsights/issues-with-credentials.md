---
title: Problemi s vjerodajnicama
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063599"
---
# <a name="issues-with-credentials"></a>Problemi s vjerodajnicama

[Microsoftova platforma za identitete i tijek vjerodajnica oauth 2,0 klijent](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) opisuje kako se program izravno protivi protoku dodjele klijentske vjerodajnice oauth 2,0.

**Kako upravljati lozinkom ili vjerodajnicama za certifikat?**

U servisu Azure CLI možete koristiti [credencijalnu aplikaciju AZ ad](https://docs.microsoft.com/cli/azure/ad/app/credential) za brisanje, popis ili vraćanje izvornih vjerodajnica aplikacija ili certifikata.

**Kako korisnici mogu ponovno postaviti lozinke?**

Korisnici se moraju [registrirati za samoposlužnu izvornu lozinku](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) da bi mogli ponovno postaviti lozinke. Kada se korisnik registrira, možete pratiti upute u ovom članku da biste ponovno postavili lozinku: [ponovno postavite lozinku za rad ili školu](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Kako korisnici mogu promijeniti svoje lozinke?**

Korisnici mogu pratiti korake u ovom članku da bi promijenili svoje lozinke: [kako promijeniti lozinku](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Mogu upravljati i [lozinkama za aplikacije za provjeru u dva koraka](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Prilikom promjene ili ponovnog postavljanja lozinke moj korisnik dobiva pogrešku**

Ta će vam veza pružiti informacije o uobičajenim problemima koji se mogu pojaviti kada korisnik pokuša ponovno postaviti lozinku: [Česti problemi i njihova rješenja](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Problem s ponovnim postavljanjem lozinke korisnika**

- Provjerite jeste li ovlašteni za ponovno postavljanje lozinki. *Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke.* Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.

- Provjerite razumijete li licencne preduvjete:

  - U vašoj tvrtki ili ustanovi mora biti dodijeljena najmanje jedna Licenca:
    - **Samo oblak korisnici** -bilo koji Office 365 (O365) Paid SKU ili Azure ad Basic
    - **Cloud i/ili lokalni korisnici** -Azure ad Premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure produktivnost Enterprise (SPE)
    - Dodatne informacije o preduvjetima za licenciranje potražite u članku [Licencne preduvjete za ponovno postavljanje lozinke za Azure ad samoposlužno](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Da biste ponovno postavili korisnikovu lozinku, pronađite korisnika u servisu Azure AD. Zatim na kartici Pregled za tog korisnika kliknite gumb "Vrati izvornu lozinku".

**Gumb za ponovno postavljanje lozinke je zasivljen**

Niste ovlašteni za ponovno postavljanje lozinki **ovog** korisnika. *Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke.* Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.

**Ne vidim oštricu za vraćanje izvorne lozinke**

Niste ovlašteni za ponovno postavljanje lozinki. *Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke.* Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.

**U odjeljku reset lozinke ne vidim članak o lokalnoj integraciji**

- Naziv lokalne integracije prikazuje se samo u hibridnim okruženjima, što znači da koristite lozinku nepotvrđenim da biste manipulirali lokalnim korisničkim lozinkama.

- Ovu oštricu ne vidite ako:

  - Ne koristite lozinku nepotvrđenim
  - Došlo je do problema s vašom instalacijom/povezivanjem lozinke za nepotvrđenim
  - Došlo je do problema s instalacijom/povezivanjem servisa Azure AD Connect
  - Dodatne upute za otklanjanje poteškoća s lozinkama za lozinke potražite u članku [Otklanjanje poteškoća s lozinkom nepotvrđenim](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Ne znam kako ponovno postaviti korisnikovu lozinku**

1. Prijavite se na portal Azure kao odgovarajući administrator.
2. Idite na sječivo **korisnika i grupe** , odaberite **Svi korisnici**.
3. Na popisu odaberite korisnika.
4. Za odabranog korisnika odaberite **Pregled**, a zatim na naredbenoj trakasti odaberite **ponovno Postavi lozinku**.
5. Odaberite gumb **Vrati izvornu lozinku** i slijedite upute na zaslonu.
    - U servisu **Azure portal** podržava se samo ponovno setovi za lozinku.

**Resetirao sam lozinku lokalnog korisnika na portalu za administratore sustava Office 365 ili mobilne aplikacije sustava Office 365, no korisnik se i dalje ne može prijaviti**

Na ovom portalu nije podržana lozinka writeback. Ponovno postavite korisnikovu lozinku na portalu Azure.
