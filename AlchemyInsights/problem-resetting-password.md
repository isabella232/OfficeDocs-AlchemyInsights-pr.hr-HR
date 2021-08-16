---
title: Problem s ponovnom postavljanjem lozinke
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
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039958"
---
# <a name="problems-resetting-password"></a>Problemi prilikom ponovnog postavljanja lozinke

Slijede neki od problema s kojima se možete sučeliti prilikom ponovnog postavljanja lozinke i mogućih rješenja:

**Imam problem s vraćanjem izvorne lozinke koji nije obuhvaćen ostalim kategorijama**

- Provjerite jeste li ovlašteni za ponovno postavljanje lozinki. Samo globalni, lozinka i administratori korisnika mogu ponovno postaviti korisničke lozinke. Globalni administratori mogu ponovno postaviti lozinke drugih administratora s ovlastima.
- Provjerite razumijete li preduvjete licenciranja:
    - Morate imati barem jednu licencu dodijeljenu u tvrtki ili ustanovi
        - Korisnici samo u oblaku – Office 365 (O365) plaćeni SKU ili Azure AD Basic
        - Korisnici u oblaku i/ili lokalnim korisnicima – Azure AD premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure Productive Enterprise (SPE)
        - Dodatne informacije o preduvjetima licenciranja potražite u članku Preduvjeti za licenciranje za samostalno ponovno postavljanje [lozinke za Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Imam problema s testiranjem pravilnika o ponovnom postavljanju lozinke koji sam postavio**

- Nedavno primijenjeni pravilnik može potrajati nekoliko minuta da bi se replicirao u svim podatkovnim centrima i krajnjim točkama. Fizička udaljenost od podatkovnog centra utječe i na brzinu primjene promjena.
- Testirajte kod krajnjeg korisnika, a ne administratora i pilotirajte s malim skupom korisnika. Pravila konfigurirana na portalu Azure odnose se samo na krajnje korisnike, a ne na administratore. Microsoft nametanje jakog zadanog pravilnika za ponovno postavljanje lozinke s dva vrata za bilo koju ulogu administratora sustava Azure (primjer: globalni administrator, administrator za podršku, administrator lozinke itd.)
    - Saznajte više o [pravilima za administratore](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Želim implementirati ponovno postavljanje lozinke, ali ne želim da korisnici registriraju dodatne sigurnosne podatke**

Unaprijed popunite podatke za korisnike da ne bi trebali! - Kao administrator možete postaviti svojstva telefona i e-pošte za korisnike prije nego što ponovno postavite lozinku u tvrtki ili ustanovi. To možete učiniti pomoću API-ja, komponente PowerShell ili azure AD Povezivanje. Dodatne informacije potražite ovdje:
- [Implementacija vraćanja izvorne lozinke bez potrebe za registracijom korisnika](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Koje podatke koristi ponovno postavljanje lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Gumb za ponovno postavljanje lozinke zasivljen je**

Niste ovlašteni ponovno postaviti korisničke lozinke. Samo globalni, lozinka i administratori korisnika mogu ponovno postaviti korisničke lozinke. Globalni administratori mogu ponovno postaviti lozinke drugih administratora s ovlastima.

**Ne vidim oštricu za ponovno postavljanje lozinke**

Niste ovlašteni za ponovno postavljanje lozinki. Samo globalni, lozinka i administratori korisnika mogu ponovno postaviti korisničke lozinke. Globalni administratori mogu ponovno postaviti lozinke drugih administratora s ovlastima.

**Ne vidim lokalni integracijski list u ponovnom postavljanju lozinke**

- Lokalni integracijski list prikazuje se samo u hibridnim okruženjima, što znači da koristite povrat lozinke za upravljanje lokalnim korisničkim lozinkama.
- Ovu oštricu ne vidite ako:
    - Ne koristite povrat pisanja lozinke
    - Došlo je do problema s instalacijom/povezivanjem povratne veze s lozinkom
    - Došlo je do problema s instalacijom/povezivanjem servisa Azure AD Povezivanje
    - Dodatne upute za otklanjanje poteškoća s vraćanjem pisanja lozinkom potražite u odjeljku Otklanjanje poteškoća [s vraćanjem pisanja lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ne znam kako ponovno postaviti korisničku lozinku**

1. Prijavite se na portal Azure kao odgovarajući administrator.
1. Idite na oštricu Korisnici i grupe, **odaberite Svi korisnici**.
1. Na popisu odaberite korisnika.
1. Za odabranog korisnika odaberite Pregled , **a** zatim na naredbenoj traci kliknite Ponovno **postavi lozinku**.
1. Slijedite upute na zaslonu.
    - Vraća se samo na izvorne postavke koje se izvode putem portala Azure, a podržavaju vraćanje lozinke.

**Ponovno postavljam lozinku lokalnog korisnika s portala Administrator sustava Office 365 ili mobilne Office 365, ali se korisnik i dalje ne može prijaviti**

Na ovom portalu nije podržano vraćanje lozinke. Ponovno postavite korisničku lozinku na portalu Azure – portal.azure.com

