---
title: Otklanjanje poteškoća s OIDC-om koji se temelje na besprijekornoj jedinstvenoj prijavi (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105759"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Otklanjanje poteškoća s OIDC-om koji se temelje na besprijekornoj jedinstvenoj prijavi (SSO)

- Da biste saznali kako dodati aplikaciju utemeljenu na OIDC-u na klijent azure, pogledajte brzi početak rada: Postavljanje jedinstvene prijave [(SSO) utemeljene na OIDC-u](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)za aplikaciju u klijentu servisa Azure Active Directory (Azure AD).
- Dodatne informacije o aplikacijama koje koriste standard OpenID Povezivanje za implementaciju jedinstvene prijave potražite u članku Razumijevanje jedinstvene prijave utemeljene na [OIDC-u](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Informacije u slučaju da odlučite napisati kod izravno slanjem i rukovanjem HTTP zahtjevima ili korištenjem biblioteke otvorenog koda drugih proizvođača, a ne pomoću jedne od naših open-source biblioteka, potražite u članku [OAuth 2.0 i OpenID Povezivanje protokoli](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)na Microsoftova platforma za identitete .

**Protokoli**

1. Microsoftova platforma za identitete i [implicitni](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) tijek dodjele – definirajući karakterističan implicitni grant jest da se tokeni (ID tokeni ili pristupni tokeni) vraćaju izravno iz krajnje točke /autoriziraj umjesto krajnje točke /tokena. To se često koristi kao dio tijeka koda za autorizaciju, u takozvanom **"hibridnom toku" –** dohvaćanje ID tokena na zahtjevu za autorizaciju uz kod za autorizaciju . U ovom se članku opisuje kako programirati izravno u protokolu u aplikaciji radi zahtjeva za tokenima od servisa Azure AD.
2. Microsoftova platforma za identitete i [OAuth 2.0 kod](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) za autorizaciju – dodjela koda za autorizaciju za OAuth 2.0 može se koristiti u aplikacijama koje su instalirane na uređaju da bi se pristupio zaštićenim resursima, kao što su WEB API-je. Pomoću Microsoftova platforma za identitete OAuth 2.0 možete dodati prijavu i **pristup API-ju u mobilne i stolne aplikacije.** U ovom se članku opisuje kako programirati izravno u protokolu u aplikaciji na bilo kojem jeziku.
3. [Microsoftova platforma za identitete i OpenID Povezivanje](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) protokol – kada koristite implementaciju programa Microsoftova platforma za identitete OpenID Povezivanje, u aplikacije možete dodati pristup aplikacijama i API-ju. U ovom se članku opisuje kako to učiniti neovisno o jeziku i opisuje kako slati i primati HTTP poruke bez korištenja **microsoftovih biblioteka** otvorenog koda .
4. Microsoftova platforma za identitete i tijek vjerodajnica klijenta za [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – možete koristiti vjerodajnice klijenta OAuth 2.0 navedene u RFC 6749, ponekad zvanom **dvonožni OAuth,** da biste pristupili resursima koje hostira web pomoću identiteta aplikacije. Ta se vrsta dodjele obično koristi za interakcije između poslužitelja i poslužitelja koje se moraju izvoditi u pozadini, bez neposredne interakcije s korisnikom. Te se vrste aplikacija često nazivaju **daemoni** ili računi **servisa**. U ovom se članku opisuje kako programirati izravno u odnosu na protokol u aplikaciji.
