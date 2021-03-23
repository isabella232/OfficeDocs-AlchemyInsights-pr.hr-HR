---
title: Otklanjanje poteškoća s protokolom OAuth 2,0 i OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035172"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Otklanjanje poteškoća s protokolom OAuth 2,0 i OpenID Connect

Da biste riješili poteškoće s povezivanjem sustava OAuth 2,0 i OpenID, izvedite sljedeće preporučene korake:

Pogledajte sljedeće članke koji su povezani s konfiguracijom i otklanjanjem poteškoća OAuth 2,0 i protokoli OpenID Connect:

- [Microsoftov identifikacijski broj platforme i OAuth 2,0 Flow kod za autorizaciju](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – u ovom se članku opisuje kako programirati izravno protiv **toka kod Granta (pkce)** u aplikaciji, pomoću bilo kojeg jezika.
- [Microsoftova platforma identiteta i tijek vjerodajnica OAuth 2,0 Client](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -u ovom se članku opisuje kako programirati izravno prema **protoku klijentske vjerodajnice** u aplikaciji.
- [Microsoftova platforma za identitete i vjerodajnice za lozinku vlasnika resursa za 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) -u ovom se članku opisuje kako programirati izravno prema **protoku ropc** u aplikaciji.
    - Platforma Microsoftova identiteta podržava samo ROPC za Azure AD stanari, a ne za osobne račune. To znači da morate koristiti krajnje točke određenog korisnika **https://login.microsoftonline.com/{TenantId_or_Name}) (** ili krajnju točku **tvrtke ili ustanove** .
    - Osobni računi pozvani na korisnika servisa Azure AD ne mogu koristiti ROPC.
    - Računi koji nemaju lozinke ne mogu se prijaviti putem servisa ROPC. U ovom scenariju preporučujemo da umjesto toga koristite različit tijek za aplikaciju.
    - Ako korisnici moraju koristiti [višestruku provjeru autentičnosti (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) da biste se prijavili u aplikaciju, bit će blokirani.
    - ROPC se ne podržava u scenarijima [hibrida identiteta](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (primjerice, Azure ad i ADFS koji se koriste za provjeru autentičnosti na lokalnim računima). Ako su korisnici putem cijele stranice preusmjereni na lokalnog davatelja identiteta, Azure AD ne može testirati korisničko ime i lozinku za tog davatelja identiteta. [Provjera autentičnosti](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) je podržana pomoću programa ropc, no.
    - Iznimka u scenariju hibridne udruge identiteta bit će sljedeće: pravilnik o otkriću u kućnom svijetu s slovom **Allowcloudpasswordvalidation** postavljen na **True** omogućit će tijek ropc-a za rad s vanjskim korisnicima kada se lokalna lozinka sinkronizira s oblacem. Dodatne informacije potražite u članku [Omogućivanje izravnog autentičnosti ROPC-ja vanjskih korisnika za naslijeđene aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Microsoftova platforma za identitete i OAuth 2,0 u programu Flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) – u ovom se članku opisuje kako programirati izravno u **tijeku tijeka rada u programu (OBO)** u aplikaciji.
- [Microsoftov identifikacijski vodič i protokol OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – u ovom se članku prikazuje kako implementirati protokol OpenID Connect nezavisno od jezika, a opisuje kako slati i primati HTTP poruke bez korištenja Microsoftovih otvorenih izvornih biblioteka.

**Pristupni tokeni**

Pomoću [Microsoftovih tokena za pristup platformama](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Informirajte se o tome kako API može provjeriti valjanost i koristiti zahtjeve u pristupnom toknu. Sva dokumentacija u ovom članku, osim ako je navedeno, primjenjuje se samo na tokene izdane za API-je koje ste registrirali. Ne primjenjuje se na tokene izdane za API-je u vlasništvu Microsofta, niti se ti tokeni mogu koristiti za provjeru načina na koji će Microsoftova platforma za identitete izdati žetone za neki API koji ste stvorili.

**Konfiguracija aplikacija**

[PREUSMJERAVANJE Uri (URL-a odgovora) ograničenja i ograničenja](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – naučite konfigurirati URI preusmjeravanja (URL za odgovaranje). URI za preusmjeravanje ili URL za odgovaranje mjesto je na kojem poslužitelj za autorizaciju šalje korisnika kada aplikacija bude uspješno ovlaštena i odobri kod za autorizaciju ili pristupni token. Poslužitelj za autorizaciju šalje kod ili token u URI preusmjeravanja; Važno je da registriramo ispravnu lokaciju kao dio postupka registracije aplikacije.

**Dodjela resursa aplikaciji**

[Praktični vodič: razvijanje i planiranje dodjele resursa za krajnju točku za scim](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) – u ovom se članku opisuje kako izgraditi scim krajnju točku i integrirati se s servisom za dodjelu resursa u AAD-u.


