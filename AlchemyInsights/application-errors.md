---
title: Pogreške aplikacije
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984518"
---
# <a name="application-errors"></a>Pogreške aplikacije

Tražite informacije o **kodovima pogrešaka Aadsts** koji se vraćaju iz servisa za sigurnost tokena za Azure Active Directory (Azure AD)? Pročitajte [lozinke za Azure ad i pogreške pri autorizaciji](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) za pronalaženje AADSTS opisa pogrešaka, popravaka i nekih predloženih zaobilaznih rješenja.

Pogreške autorizacije mogu biti rezultat nekoliko različitih problema, od kojih većina generira pogrešku 401 ili 403. Na primjer, sljedeće može dovesti do pogrešaka autorizacije:

- Netočni [Tijekovi nabave za pristup tokena](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Slabo konfigurirane [dosege dozvola](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Da biste riješili uobičajene pogreške autorizacije, isprobajte upute navedene u nastavku koje najviše odgovaraju pogrešci koju primate. Može se primijeniti više od jednog.

**401 neovlašteno pogreške: je li vaš token valjan?**

Pobrinite se da aplikacija prikazuje valjani token za Access u programu Microsoft Graph kao dio zahtjeva. Ta pogreška često znači da možda nema tokena programa Access u zaglavlju zahtjeva za HTTP provjeru autentičnosti ili da token nije valjan ili je istekao. Preporučujemo da koristite [Microsoftovu biblioteku za provjeru autentičnosti (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) za nabavu tokena programa Access. Uz to, ta se pogreška može pojaviti ako pokušate koristiti ovlašteni pristupni token dodijeljen osobnom Microsoftovu računu za pristup API-ju koji podržava samo račune tvrtke ili obrazovne ustanove (poslovni računi).

**403 zabranjena pogreška: Jeste li odabrali odgovarajući skup dozvola?**

Provjerite jeste li zatražili ispravni skup dozvola na temelju programa Microsoft Graph za API-je u aplikaciji. Preporučene najmanje privilegirane dozvole osiguravaju se u svim temama metoda referenca za Microsoft Graph API. Uz to, korisnik ili administrator moraju dodijeliti te dozvole aplikaciji. Dodjela dozvola obično se događa putem stranice pristanka ili dopuštanjem dozvola pomoću servisa za registraciju aplikacije za Azure portal. Na kartici **Postavke** za aplikaciju kliknite **obavezne dozvole**, a zatim kliknite **Dodjela dozvola**.

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumijevanje dozvola i pristanka za Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 zabranjena pogreška: je li vaša aplikacija stekla token za podudaranje odabranih dozvola?**

Provjerite odgovara li vrsta dozvola koja se traži ili dodjeljuje vrsti pristupnog tokena koji aplikacija preuzima. Možda zatražite i dodijelite dozvole za aplikacije, ali pomoću tokena za prijenos interaktivnih kodova, umjesto tokena protoka vjerodajnica za klijente, ili zatražite i dodijelite delegirane dozvole, ali pomoću žetona tijeka rada za klijentske vjerodajnice, umjesto tokena za strujanje kodova.

- [Dohvaćanje pristupa u ime korisnika i delegiranih dozvola](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-OAuth 2,0 funkcija koda za autorizaciju](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Dohvaćanje programa Access bez korisničke dozvole i dozvola za aplikacije](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0-OAuth 2,0 Client vjerodajnice Flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 zabranjena pogreška: ponovno postavljanje lozinke**

Trenutno ne postoje dozvole za aplikaciju daemon servis za servis koji omogućuju vraćanje korisničkih lozinki. Ovi API podržani su samo pomoću interaktivnog delegiranog koda koji teče s administratorskim administratorom.

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 je zabranjen: ima li korisnik pristup i jesu li licencirani?**

Ako je za delegirani broj tokova, Microsoft Graph ocjenjuje je li zahtjev dopušten na temelju dozvola dodijeljenih aplikaciji i dozvola koje korisnik prijave sadrži. Ova pogreška općenito upućuje na to da korisnik nije dovoljno privilegiran da izvrši zahtjev ili da korisnik nije licenciran za pristup podacima. Zahtjev može uspješno izvršiti samo korisnici s obaveznom dozvolom ili licencama.

**403 je zabranjen: Jeste li odabrali ispravan API resursa?**

API servisi kao što je Microsoft Graph potvrdit će da je dodatak AUD (publika) u primljenom pristupnom toklu odgovara vrijednosti koju očekuje, a ako ne, rezultat je u zabranjenoj pogrešci 403. Najčešća pogreška koja je prouzročena tom pogreškom pokušava upotrijebiti token za Azure AD Graph API, Outlook APIs ili SharePoint/OneDrive API-je za pozivanje programa Microsoft Graph (ili obratno). Pobrinite se da resurs (ili doseg) aplikacija nabavi token za podudaranje sa API-jem koji aplikacija poziva.

**400 loš zahtjev ili 403 zabranjen: primjenjuje li se korisnik u pravilima uvjetnog pristupa (CA) tvrtke ili ustanove?**

Na temelju Pravilnika tvrtke ili ustanove, korisnik koji pristupi resursima programa Microsoft Graph putem aplikacije možda će izazvati dodatne informacije koje nisu prisutne u Tokenu programa Access koju je vaša aplikacija prvobitno stekla. U ovom slučaju aplikacija sadrži 400 s pogreškom *interaction_required* tijekom nabave tokena programa access ili 403 s pogreškama *Insufficient_claims* prilikom pozivanja programa Microsoft Graph. U oba slučaja odgovor na pogrešku sadrži dodatne informacije koje se mogu prikazati u krajnjoj točki autorizacije da biste korisniku izazvali dodatne informacije (kao što su multi-Factor provjera autentičnosti ili uvrštenja uređaja).

- [Rukovanje izazovima uvjetnog pristupa pomoću MSAL-a ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Upute za razvojne inženjere u uvjetnom pristupu servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
