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
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931441"
---
# <a name="application-errors"></a>Pogreške aplikacije

Tražite informacije o kodovima **pogrešaka AADSTS** koji se vraćaju iz servisa za sigurnosne tokene sustava Azure Active Directory (Azure AD) (AZURE AD) (STS)? Pročitajte [kodove za provjeru autentičnosti](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) i autorizaciju servisa Azure AD da biste pronašli opise pogrešaka, popravke i neka predložena zaobilazna rješenja.

Pogreške u autorizaciji mogu biti rezultat nekoliko različitih problema, od kojih većina generira pogrešku 401 ili 403. Sljedeće, primjerice, može dovesti do pogrešaka u autorizaciji:

- Netočni [tijekovi prikupljanja pristupnog tokena](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Loše konfigurirani [opsezi dopuštenja](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Da biste riješili uobičajene pogreške u autorizaciji, isprobajte korake navedene u nastavku da se najčešće podudaraju s pogreškom koju primate. Može se primijeniti više od jednog.

**401 Neovlaštena pogreška: Je li vaš token valjan?**

Provjerite predstavlja li vaša aplikacija valjani token za pristup microsoftu Graph kao dio zahtjeva. Ova pogreška često znači da pristupni token možda nedostaje u zaglavlju zahtjeva za provjeru autentičnosti HTTP-a ili da je token nevaljan ili je istekao. Preporučujemo da koristite Microsoftovu biblioteku provjere [autentičnosti (MSAL) za preuzimanje](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) tokena za pristup. Osim toga, ta se pogreška može pojaviti ako pokušate koristiti token za delegirani pristup dodijeljen osobnom Microsoftovu računu za pristup API-ju koji podržava samo poslovne ili školske račune (račune tvrtke ili ustanove).

**403 Zabranjena pogreška: Jeste li odabrali pravi skup dozvola?**

Provjerite jeste li zatražili točan skup dozvola na temelju API-ja Graph aplikacije. Preporučene dozvole s najmanjim privilegijama navedene su u svim temama Graph metode referenci za Microsoft Graph API. Uz to, ta dopuštenja aplikaciji mora dodijeliti korisnik ili administrator. Dodjela dozvola obično se događa putem stranice za pristanak ili dodjelom dozvola pomoću registracijskog lista aplikacije Azure Portal. U odjeljku **Postavke** za aplikaciju kliknite **Potrebna dopuštenja**, a zatim kliknite na **Dodijeli dozvole za**.

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumijevanje dozvola i pristanka za Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Zabranjena pogreška: Je li vaša aplikacija stekla token koji odgovara odabranim dozvolama?**

Provjerite podudara li se vrsta zatraženih ili odobrenih dozvola s vrstom pristupnog tokena koju vaša aplikacija nabavlja. Možda zatražite i dodjeljujete dozvole za aplikacije, ali umjesto tokena tijeka klijentskih vjerodajnica koristite delegirane interaktivne tokene tijeka koda ili zatražite i dodijelite delegirane dozvole, ali umjesto tokena tijeka delegiranog koda koristite tokene tijeka klijentskih vjerodajnica.

- [Pristupite u ime korisnika i delegiranih dozvola](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 – tijek koda za autorizaciju OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Pristupite bez korisnika (usluga demona) i dopuštenja aplikacije](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 – Tijek vjerodajnica klijenta OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Zabranjena pogreška: Resetiranje lozinke**

Trenutno ne postoje dozvole za korištenje daemon servisa za aplikacije koja omogućuju poništavanje korisničkih lozinki. Ovi API-ji podržani su samo pomoću interaktivnih tijekova delegiranog koda s prijavljenim administratorom.

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 Zabranjeno: Ima li korisnik pristup i ima li licencu?**

Za delegirane tokove koda Microsoft Graph procjenjuje je li zahtjev dopušten na temelju dozvola dodijeljenih aplikaciji i dozvola koje ima prijavljeni korisnik. Općenito, ova pogreška ukazuje na to da korisnik nije dovoljno privilegiran da izvrši zahtjev ili da nema licencu za podatke kojima se pristupa. Samo korisnici s potrebnim dozvolama ili licencama mogu uspješno podnijeti zahtjev.

**403 Zabranjeno: Jeste li odabrali ispravan API resursa?**

API servisi kao što je Microsoft Graph provjerava podudaraju li se zvučni zahtjev (ciljna publika) u primljenom tokenu za pristup vrijednosti koju očekuje za sebe, a ako ne, to rezultira pogreškom 403 Forbidden. Uobičajena pogreška koja rezultira ovom pogreškom je pokušaj upotrebe tokena stečenog za API-je Azure AD Graph, Outlook API-je ili SharePoint / OneDrive API-je za pozivanje Microsoft Graph-a (ili obrnuto). Osigurajte da resurs (ili opseg) vaše aplikacije stječe token za podudaranje s API-jem koji aplikacija poziva.

**400 loš zahtjev ili 403 zabranjeno: pridržava li se korisnik pravila uvjetnog pristupa (CA) svoje organizacije?**

Na temelju pravilnika za ovjeravanje tvrtke ili ustanove korisnik koji pristupa resursima sustava Microsoft Graph putem vaše aplikacije može biti osporen radi dodatnih informacija koje nisu prisutne u tokenu za pristup koji je vaša aplikacija izvorno nabavila. U ovom slučaju, vaša aplikacija prima 400 s *pogreškom interaction_required* tijekom nabave pristupnog tokena ili 403 s pogreškom *insufficient_claims* prilikom pozivanja servisa Microsoft Graph. U oba slučaja odgovor na pogreške sadrži dodatne informacije koje se mogu prikazati krajnjoj točki ovlaštenja radi izazivanja korisnika radi dodatnih informacija (kao što su višestruka provjera autentičnosti ili registracija uređaja).

- [Rješavanje izazova uvjetnog pristupa pomoću MSAL-a ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Smjernice za programere za uvjetni pristup Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
