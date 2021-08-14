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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986811"
---
# <a name="issues-with-credentials"></a>Problemi s vjerodajnicama

Microsoftova platforma za identitete i tijek vjerodajnica klijenta [za OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) opisuje kako programirati izravno u odnosu na klijentske vjerodajnice za OAuth 2.0.

**Kako upravljati lozinkom ili vjerodajnicama certifikata aplikacije?**

Na servisu Azure CLI vjerodajnice aplikacije [az ad možete](https://docs.microsoft.com/cli/azure/ad/app/credential) koristiti za brisanje, popis ili vraćanje izvorne lozinke ili vjerodajnica certifikata aplikacije.

**Kako korisnici mogu ponovno postaviti lozinke?**

Korisnici se moraju registrirati [za samostalno ponovno postavljanje lozinke](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) da bi mogli ponovno postaviti lozinke. Kada se korisnik registrira, može slijediti upute u ovom članku da bi ponovno postavili lozinku: ponovno [postavite lozinku tvrtke ili škole.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Kako korisnici mijenjaju lozinke?**

Korisnici mogu slijediti korake u ovom članku da bi promijenili lozinke: [Kako promijeniti lozinku](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Mogu i upravljati [lozinkama za aplikacije za provjeru valjanosti u dva koraka](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Prilikom promjene ili ponovnog postavljanja lozinke korisniku se prikazuje pogreška**

Ta će veza pružiti informacije o uobičajenim problemima koji se mogu pojaviti kada korisnik pokušava ponovno postaviti lozinku: [uobičajeni problemi i njihova rješenja](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Imam problem s vraćanjem korisnikova lozinke**

- Provjerite jeste li ovlašteni za ponovno postavljanje lozinki. *Samo globalni, lozinka i administratori korisnika mogu ponovno postaviti korisničke lozinke.* Globalni administratori mogu ponovno postaviti lozinke drugih administratora s ovlastima.

- Provjerite razumijete li preduvjete za licenciranje:

  - Morate imati barem jednu licencu dodijeljenu u tvrtki ili ustanovi:
    - **Korisnici samo u oblaku** – Office 365 (O365) plaćeni SKU ili Azure AD Basic
    - **Korisnici u oblaku i/ili** lokalnim korisnicima – Azure AD premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure Productive Enterprise (SPE)
    - Dodatne informacije o preduvjetima licenciranja potražite u članku Preduvjeti za licenciranje za samostalno ponovno [postavljanje lozinke za Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Da biste ponovno postavili korisničku lozinku, pronađite korisnika na servisu Azure AD. Zatim na oštrici pregleda za tog korisnika kliknite gumb "ponovno postavi lozinku".

**Gumb za ponovno postavljanje lozinke zasivljen je**

Niste ovlašteni ponovno postaviti **korisničke** lozinke. *Samo globalni, lozinka i administratori korisnika mogu ponovno postaviti korisničke lozinke.* Globalni administratori mogu ponovno postaviti lozinke drugih administratora s ovlastima.

**Ne vidim oštricu za ponovno postavljanje lozinke**

Niste ovlašteni za ponovno postavljanje lozinki. *Samo globalni, lozinka i administratori korisnika mogu ponovno postaviti korisničke lozinke.* Globalni administratori mogu ponovno postaviti lozinke drugih administratora s ovlastima.

**Ne vidim lokalni integracijski list u ponovnom postavljanju lozinke**

- Lokalni integracijski list prikazuje se samo u hibridnim okruženjima, što znači da koristite povrat lozinke za upravljanje lokalnim korisničkim lozinkama.

- Ovu oštricu ne vidite ako:

  - Ne koristite povrat pisanja lozinke
  - Došlo je do problema s instalacijom/povezivanjem povratne veze s lozinkom
  - Došlo je do problema s instalacijom/povezivanjem servisa Azure AD Povezivanje
  - Dodatne upute za otklanjanje poteškoća s povratom pisanja lozinkom potražite u članku Otklanjanje [poteškoća s vraćanjem pisanja lozinke](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Ne znam kako ponovno postaviti korisničku lozinku**

1. Prijavite se na portal Azure kao odgovarajući administrator.
2. Idite na **oštricu Korisnici i grupe,** **odaberite Svi korisnici**.
3. Na popisu odaberite korisnika.
4. Za odabranog korisnika odaberite Pregled , **a** zatim na naredbenoj traci odaberite Ponovno **postavi lozinku**.
5. Odaberite **gumb Ponovno postavi** lozinku i slijedite upute na zaslonu.
    - Vraća se samo na izvorne postavke koje se izvode putem **portala Azure, a** podržavaju vraćanje lozinke.

**Ponovno postavljam lozinku lokalnog korisnika s portala Administrator sustava Office 365 ili mobilne Office 365, ali se korisnik i dalje ne može prijaviti**

Na ovom portalu nije podržano vraćanje lozinke. Ponovno postavite korisničku lozinku na portalu Azure.
