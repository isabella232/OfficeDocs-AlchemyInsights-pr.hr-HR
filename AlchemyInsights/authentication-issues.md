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
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976841"
---
# <a name="authentication-issues"></a>Problemi s provjerom autentičnosti

**Tražite informacije o AADSTS kodovima pogrešaka koji se vraćaju iz usluge sigurnosnih tokena Azure Active Directory (Azure AD)?** Pogledajte članak [Azure AD autentifikacija i kodovi pogrešaka za autorizaciju ](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)da biste pronašli opise pogrešaka, ispravke i neke predložene zaobilazne načine AADSTS.

Pogreške u autorizaciji mogu biti rezultat nekoliko različitih problema, od kojih većina generira pogrešku 401 ili 403. Na primjer, sljedeći problemi mogu dovesti do pogrešaka u autorizaciji:

- Netočni [tijekovi prikupljanja pristupnog tokena](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Loše konfigurirani [opsezi dopuštenja](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Da biste riješili uobičajene pogreške autorizacije, isprobajte korake navedene u nastavku koji se najviše podudaraju s pogreškom koju primate. Više koraka može se primijeniti za pogrešku koju primate.

**401 Neovlaštena pogreška: Je li vaš token valjan?**

Provjerite prikazuje li vaša aplikacija valjani pristupni token Microsoft Graphu kao dio zahtjeva. Ova pogreška često znači da pristupni token možda nedostaje u zaglavlju zahtjeva za provjeru autentičnosti HTTP-a ili da je token nevaljan ili je istekao. Preporučujemo vam da koristite Microsoft Authentication Library (MSAL) za prikupljanje pristupnih tokena. Uz to, ova se pogreška može dogoditi ako pokušate upotrijebiti token za delegirani pristup dodijeljen osobnom Microsoftovom računu za pristup API-ju koji podržava samo radne ili školske račune (organizacijski računi).

**403 Zabranjena pogreška: Jeste li odabrali pravi skup dozvola?**

Provjerite jeste li zatražili ispravan skup dozvola na temelju API-ja Microsoft Graph koji vaša aplikacija poziva. Preporučena najmanje privilegirana dopuštenja nalaze se u svim temama referentne metode Microsoft Graph API. Uz to, ta dopuštenja aplikaciji mora dodijeliti korisnik ili administrator. Dodjela dozvola obično se događa putem stranice saglasnosti ili korištenja oštrice za registraciju aplikacije Azure Portal. U odjeljku **Postavke** za aplikaciju kliknite **Potrebna dopuštenja**, a zatim kliknite na **Dodijeli dozvole za**. Dodatne informacije potražite u članku:

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumijevanje dozvola i pristanka za Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Zabranjena pogreška: Je li vaša aplikacija stekla token koji odgovara odabranim dozvolama?**

Provjerite podudaraju li se vrste odobrenih ili dodijeljenih dozvola vrsti pristupnog tokena koji vaša aplikacija stječe. Možda zatražite i odobrite dozvole za aplikacije, ali koristite delegirane interaktivne tokene toka koda umjesto tokena protoka vjerodajnica klijenta ili tražite i dodijelite delegirana dopuštenja, ali koristite tokene tijeka vjerodajnica klijenta umjesto delegiranih tokena tijeka koda.

Dodatne informacije o stjecanju tokena, potražite u članku:

- [Pristupite u ime korisnika i delegiranih dozvola](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 – tijek koda za autorizaciju OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Pristupite bez korisnika (usluga demona) i dopuštenja aplikacije](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 – Tijek vjerodajnica klijenta OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Zabranjena pogreška: Resetiranje lozinke**

Trenutno ne postoje dozvole za korištenje daemon servisa za aplikacije koja omogućuju poništavanje korisničkih lozinki. Ovi API-ji podržani su samo pomoću interaktivnih tijekova delegiranog koda s prijavljenim administratorom. Dodatne informacije potražite u članku [Microsoft Graph dozvole](https://docs.microsoft.com/graph/permissions-reference).

**403 Zabranjeno: Ima li korisnik pristup i ima li licencu?**

Za tijekove delegiranog koda, Microsoft Graph procjenjuje je li zahtjev dopušten na temelju dozvola dodijeljenih aplikaciji i dopuštenja koja ima prijavljeni korisnik. Općenito, ova pogreška ukazuje na to da korisnik nije dovoljno privilegiran da izvrši zahtjev **ili** da nema licencu za podatke kojima se pristupa. Samo korisnici s potrebnim dozvolama ili licencama mogu uspješno podnijeti zahtjev.

**403 Zabranjeno: Jeste li odabrali ispravan API resursa?**

API usluge kao što je Microsoft Graph provjeravaju da li zahtjev *audijencije* (publika) u pristupnom tokenu odgovara vrijednosti koju očekuje za sebe, a ako ne, dogodi se zabranjena pogreška 403. Uobičajena pogreška koja rezultira ovom pogreškom je pokušaj upotrebe tokena stečenog za API-je Azure AD Graph, Outlook API-je ili SharePoint / OneDrive API-je za pozivanje Microsoft Graph-a (ili obrnuto). Osigurajte da resurs (ili opseg) vaše aplikacije stječe token za podudaranje s API-jem koji aplikacija poziva.

**400 loš zahtjev ili 403 zabranjeno: pridržava li se korisnik pravila uvjetnog pristupa (CA) svoje organizacije?**

Na temelju pravila uvjetnog pristupa (CA) organizacije, korisnik koji pristupa resursima Microsoft Graph-a putem vaše aplikacije može biti osporavan zbog dodatnih podataka koji nisu prisutni u tokenu pristupa koji je vaša aplikacija prvobitno stekla. U ovom slučaju, vaša aplikacija prima **400 s *pogreškom interaction_required*** tijekom nabave pristupnog tokena ili **403 s pogreškom *insufficient_claims*** prilikom pozivanja servisa Microsoft Graph. U oba slučaja odgovor na pogrešku sadrži dodatne informacije koje se mogu predstaviti ovlaštenoj krajnjoj točki kako bi se korisnici pozvali na dodatne informacije (poput višefaktorske autentifikacije ili registracije uređaja).

Dodatne informacije vezane uz uvjetni pristup, potražite u članku:

- [Rukovanje izazovima uvjetnog pristupa pomoću MSAL-a](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Smjernice za programere za uvjetni pristup Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Kraj podrške za Azure Active Directory Authentication Library (ADAL) i Azure AD Graph API (AAD Graph)_* _

- Od 30. lipnja 2020. više nećemo dodavati nove značajke u Azure Active Directory Authentication Library (ADAL) i Azure AD Graph API (AAD Graph). I dalje ćemo pružati tehničku podršku i sigurnosna ažuriranja, ali više nećemo pružati ažuriranja značajki.
- Od 30. lipnja 2022. ukinut ćemo podršku za ADAL i AAD Graph i više nećemo pružati tehničku podršku ili sigurnosna ažuriranja.
    - Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće dobiti nikakvu tehničku podršku ili sigurnosna ažuriranja.
    - Aplikacije koje koriste AAD Graph nakon tog vremena možda više neće primati odgovore od krajnje točke AAD Graph.

_ *ADAL migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) koja ima najnovije značajke i sigurnosna ažuriranja. Ova je preporuka u kontekstu Microsoftove migracije svojih aplikacija na MSAL do krajnjeg roka za podršku. Cilj migracije Microsoftovih aplikacija na MSAL je osigurati da aplikacije imaju koristi od stalnih poboljšanja MSAL-a i značajki.

- [Pročitajte najčešća pitanja vezana za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Saznajte kako migrirati aplikacije na platformu](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Ako trebate pomoć u razumijevanju koja od vaših aplikacija koristi ADAL, preporučujemo vam da pregledate izvorni kod svih aplikacija i ako je primjenjivo obratite se neovisnim dobavljačima softvera (ISV-ovima) ili pružateljima aplikacija. Microsoftova podrška također vam može pružiti popis svih aplikacija koje nisu Microsoftove ADAL u vašem klijentu.

**Migracija grafikona AAD**

Za aplikacije koje koriste AAD Graph, slijedite naše smjernice za [migriranje aplikacija Azure AD Graph na Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Naš popis za migraciju pruža točku početka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Vaš portal za registraciju Azure aplikacija prikazuje koje aplikacije koriste AAD Graph. Preporučujemo da pregledate izvorni kod svih aplikacija i ako je primjenjivo obratite se svim ISV-ovima ili davateljima aplikacija. Microsoftova podrška također vam može pružiti informacije o cijeloj upotrebi AAD Graph u vašem stanaru.

 










