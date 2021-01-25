---
title: Problemi s provjerom autentičnosti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974234"
---
# <a name="authentication-issues"></a>Problemi s provjerom autentičnosti

**Tražite informacije o kodovima pogrešaka AADSTS koji se vraćaju iz servisa za sigurnost tokena za Azure Active Directory (Azure AD)?** Pročitajte članak [lozinke za Azure ad i pogreške pri autorizaciji](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) za pronalaženje AADSTS opisa pogrešaka, popravaka i nekih predloženih zaobilaznih rješenja.

Pogreške autorizacije mogu biti rezultat nekoliko različitih problema, od kojih većina generira pogrešku 401 ili 403. Na primjer, sljedeći problemi mogu dovesti do pogrešaka autorizacije:

- Netočni [Tijekovi nabave za pristup tokena](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Slabo konfigurirane [dosege dozvola](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Da biste riješili uobičajene pogreške autorizacije, isprobajte upute navedene u nastavku koje najviše odgovaraju pogrešci koju primate. Za pogrešku koju primate može se primijeniti više koraka.

- **401 neovlašteno pogreške: je li vaš token valjan?**

Pobrinite se da aplikacija prikazuje valjani token za Access u programu Microsoft Graph kao dio zahtjeva. Ta pogreška često znači da možda nema tokena programa Access u zaglavlju zahtjeva za HTTP provjeru autentičnosti ili da token nije valjan ili je istekao. Preporučujemo da koristite Microsoftovu biblioteku za provjeru autentičnosti (MSAL) za nabavu tokena programa Access. Uz to, ta se pogreška može pojaviti ako pokušate koristiti delegirani pristupni token dodijeljen osobnom Microsoftovu računu za pristup API-ju koji podržava samo račune tvrtke ili obrazovne ustanove.

**403 zabranjena pogreška: Jeste li odabrali odgovarajući skup dozvola?**

Provjerite jeste li zatražili ispravni skup dozvola na temelju programa Microsoft Graph za API-je u aplikaciji. Preporučene najmanje privilegirane dozvole osiguravaju se u svim temama metoda referenca API-ja za Microsoft Graph. Uz to, korisnik ili administrator moraju dodijeliti te dozvole aplikaciji. Dodjela dozvola obično se događa putem stranice pristanka ili korištenja noža za registraciju aplikacije Azure portal. Na kartici **Postavke** za aplikaciju kliknite **obavezne dozvole**, a zatim kliknite **Dodjela dozvola**. Dodatne informacije potražite u članku:

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumijevanje dozvola i pristanka za Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 zabranjena pogreška: je li vaša aplikacija stekla token za podudaranje odabranih dozvola?**

Uvjerite se da su vrste dozvola zatražene ili dodijeljene podudarne s vrstom pristupnog tokena koju aplikacija preuzima. Možda zatražite i dodijelite dozvole za aplikacije, ali pomoću tokena za prijenos interaktivnih kodova, umjesto tokena protoka vjerodajnica za klijentski pristup, zatražite i dodijelite delegirane dozvole, a ne želite da se tokeni protočni točni kodovi nalaze na karticama.

Dodatne informacije vezane uz stjecanje tokena potražite u članku:

- [Dohvaćanje pristupa u ime korisnika i delegiranih dozvola](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-OAuth 2,0 funkcija koda za autorizaciju](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Dohvaćanje programa Access bez korisničke dozvole i dozvola za aplikacije](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0-OAuth 2,0 Client vjerodajnice Flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 zabranjena pogreška: ponovno postavljanje lozinke**

Trenutno ne postoje dozvole za aplikaciju daemon servis za servis koji omogućuju vraćanje korisničkih lozinki. Ovi API podržani su samo pomoću interaktivnog delegiranog koda koji teče s administratorskim administratorom. Dodatne informacije potražite u članku [dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 je zabranjen: ima li korisnik pristup i jesu li licencirani?**

Ako je za delegirani broj tokova, Microsoft Graph procjenjuje je li zahtjev dopušten na temelju dozvola dodijeljenih aplikaciji i dozvolama koje je korisnik potpisao. Ova pogreška općenito upućuje na to da korisnik nije dovoljno privilegiran da izvrši zahtjev **ili** da korisnik nije licenciran za pristup podacima. Zahtjev može uspješno izvršiti samo korisnici s obaveznom dozvolom ili licencama.

**403 je zabranjen: Jeste li odabrali ispravan API resursa?**

API servisi kao što je Microsoft Graph *potvrdit će* da u primljenom pristupnom toklu odgovara vrijednost koju očekuje, a ako ne, pojavljuje se pogreška 403. Najčešća pogreška koja je prouzročena tom pogreškom pokušava upotrijebiti token za Azure AD Graph API, Outlook APIs ili SharePoint/OneDrive API-je za pozivanje programa Microsoft Graph (ili obratno). Pobrinite se da resurs (ili doseg) aplikacija nabavi token za podudaranje sa API-jem koji aplikacija poziva.

**400 loš zahtjev ili 403 zabranjen: primjenjuje li se korisnik u pravilima uvjetnog pristupa (CA) tvrtke ili ustanove?**

Na temelju Pravilnika o uvjetnom pristupu (CA) tvrtke ili ustanove, korisnik koji je pristupio resursima programa Microsoft Graph putem aplikacije može izazvati dodatne informacije koje nisu prisutne u token programa Access koju je vaša aplikacija prvobitno stekla. U ovom slučaju aplikacija sadrži **400 s pogreškom *interaction_required*** tijekom nabave tokena programa Access ili **403 s pogreškama *insufficient_claims*** prilikom pozivanja programa Microsoft Graph. U oba slučaja odgovor na pogrešku sadrži dodatne informacije koje je moguće prikazati u ovlaštenoj krajnjoj točki da biste korisniku izazvali dodatne informacije (kao što su višestruka provjera autentičnosti ili uvrštenja uređaja).

Dodatne informacije vezane uz uvjetni pristup potražite u članku:

- [Rukovanje izazovima uvjetnog pristupa pomoću MSAL-a](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Upute za razvojne inženjere u uvjetnom pristupu servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Kraj podrške za Azure Active Directory za biblioteku autentičnosti (ADAL) i Azure ad Graph API (AAD Graph)_* _

- Počevši od 30 Lipanj, 2020, više nećemo dodavati nove značajke u biblioteku servisa Azure Active Directory za provjeru autentičnosti (ADAL) i API-ja za Azure AD Graph (AAD Graph). Nastavit ćemo pružati tehničku podršku i sigurnosno ažuriranje, ali više nećemo pružati ažuriranja značajki.
- Počevši od 30 lipnja 2022, završit ćemo podršku za ADAL i AAD Graph i više neće pružati tehničku podršku ni Sigurnosno ažuriranje.
    - Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće dobiti nikakvu tehničku podršku ni Sigurnosno ažuriranje.
    - Aplikacije koje koriste AAD Graph nakon tog vremena možda više neće primati odgovore iz krajnje točke AAD grafikona.

_ *Adal migracija**

Preporučujemo ažuriranje [Microsoftove biblioteke za provjeru autentičnosti (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), koja sadrži najnovije značajke i sigurnosno ažuriranje. Ta je preporuka u kontekstu programa Microsoft Migriranje svojih aplikacija u MSAL uz krajnji rok za podršku. Cilj migracije Microsoftovih aplikacija u MSAL jest osigurati da se aplikacije koristi u trenutnoj sigurnosti i poboljšanjima značajki MSAL-a.

- [Pročitajte najčešća pitanja o dodatku](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Informacije o migraciji aplikacija na temelju osnove platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL, preporučujemo vam da pregledate sve izvorne šifre aplikacija i ako je primjenjivo, Dopratite sve nezavisne dobavljače softvera (ISVs) ili davatelja aplikacija. Microsoftova podrška može vam pružiti i popis svih aplikacija koje nisu Microsoftove ADAL u vašem zakupcu.

**Migracije grafikona AAD**

Za aplikacije koje koriste AAD Graph, slijedite upute da biste [migrirali aplikacije Azure ad Graph u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Naš popis za migraciju sadrži točku početka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Portal za registraciju servisa Azure sadrži programe koje koristi AAD Graph. Preporučujemo vam da pregledate sve izvorne šifre aplikacija, a ako je primjenjivo, obratite se svim pružateljima programa ISVs ili aplikacije. Microsoftova podrška može vam pružiti i informacije o korištenju svih AAD grafikona u vašem zakupcu.

 










