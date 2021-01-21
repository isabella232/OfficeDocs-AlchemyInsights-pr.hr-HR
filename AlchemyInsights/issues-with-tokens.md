---
title: Problemi s tokena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916694"
---
# <a name="issues-with-tokens"></a>Problemi s tokena

Da biste upravljali problemima koji se odnose na tokene, možete poduzeti sljedeće korake:

1. Možete navesti životni vijek programa Access, ID ili SAML koji je izdala Microsoftova osobna platforma. U svim aplikacijama u vašoj tvrtki ili ustanovi možete postaviti znak trajanja tokena, za višečlansku (multi-organizacijsku) aplikaciju ili za određenog upravitelja servisa u vašoj tvrtki ili ustanovi. Dodatne informacije potražite u članku [podesiva funkcija tokena u Microsoftovoj platformi Identity (pretpregled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Tokeni programa Access omogućuju klijentima da sigurno nazovu zaštićene web-API-je, a pomoću njih web-API obavljaju provjeru autentičnosti i autorizaciju. Prema specifikacijama OAuth, pristupni tokeni su neprozirni string bez skupa oblika – Neki davatelji identiteta (IDPs) koriste GUID-ove, a drugi koriste šifrirane mrljica. Microsoftova platforma za identitete koristi razne oblike tokena programa Access, ovisno o konfiguraciji API-ja koji prihvaća token. Da biste doznali kako API može provjeriti valjanost i koristiti zahtjeve u pristupnom toknu, pročitajte članak [tokeni za pristup tvrtki Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Biblioteka programa Microsoft Authentication (MSAL) podržava nekoliko tokova provjere autentičnosti za korištenje u različitim scenarijima aplikacija. Dodatne informacije potražite u članku [tijek provjere autentičnosti](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Deautorizacija koda OAuth 2,0 može se koristiti u aplikacijama koje su instalirane na uređaju radi pristupa zaštićenim resursima, kao što je web-API. Pomoću Microsoftove platforme za identitete sustava OAuth 2,0 možete dodati pristup prijave i API-ja na mobilne i aplikacije za stolna računala. Pročitajte članak [Microsoft Identity Platform i OAuth 2,0 za autorizaciju koda](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) za programiranje izravno na protokolu u aplikaciji, pomoću bilo kojeg jezika.
5. OpenID Connect (OIDC) je protokol za provjeru autentičnosti izgrađen na OAuth 2,0 koji možete koristiti za sigurno prijavljivanje korisnika u aplikaciju. Kada koristite aplikaciju OpenID Connect u krajnje točke Microsoftove platforme za identifikaciju, možete dodati pristup prijave i API-ja u svoje aplikacije. [Microsoftov identitet Platform i OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) pokazuje kako to učiniti nezavisnim jezikom i opisuje kako slati i primati HTTP poruke bez korištenja bilo koje Microsoftove biblioteke otvorenog izvora.
    - Krajnja točka UserInfo dio je standarda OIDC, dizajniran za povrat potraživanja o korisniku koji je ovjeren. Dodatne informacije potražite u [članku krajnji Point UserInfo platforme Microsoftova identiteta](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - Naziv [web-API-ja u web-aplikaciji pomoću Azure ad i OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) uzorka prikazuje kako izgraditi MVC web-aplikaciju koja koristi Azure ad za prijavu pomoću protokola OpenID Connect, a zatim poziv na web-API u identitetu korisnika koji je potpisao pomoću tokena dobivenih putem OAuth 2,0. U ovom se uzorku koristi OpenID Connect ASP .net OWIN middleware i ADAL .net.
6. [Konfigurirajte aplikaciju koja će izložiti web-API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -u ovom Quickstart, registrirajte web-API pomoću Microsoftove platforme za identitete i Izložit ćete ga klijentskim aplikacijama dodavanjem primjera dosega. Registriranjem web-API-ja i izlaganjem putem dosega možete pružati pristup njegovim resursima ovlaštenim korisnicima i klijentskim aplikacijama koje pristupaju API-ju.
7. U servisu Azure Active Directory B2C (Azure AD B2C), unos vjerodajnica za lozinku vlasnika resursa (ROPC) predstavlja standardnu provjeru autentičnosti. U ovom protoku aplikacija, poznata i kao stranačka stranka, razmjenjuje valjane vjerodajnice za žetone. Vjerodajnice sadrže korisnički ID i lozinku. Vraćeni žetoni jesu ID token, token za Access i token osvježavanja. Dodatne informacije potražite u odjeljku [Postavljanje tijeka vjerodajnice za lozinku vlasnika resursa u servisu Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

