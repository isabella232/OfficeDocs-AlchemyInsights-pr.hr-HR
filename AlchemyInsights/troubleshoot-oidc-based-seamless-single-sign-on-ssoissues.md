---
title: Otklanjanje poteškoća vezanih uz jedinstvenu prijavu (SSO) na temelju OIDC-a
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
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743452"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Otklanjanje poteškoća vezanih uz jedinstvenu prijavu (SSO) na temelju OIDC-a

- Upute za dodavanje aplikacije temeljene na OIDC-u klijentu za Azure [: postavljanje jedinstvene prijave za aplikaciju OIDC (SSO) u servisu Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- Dodatne informacije o aplikacijama koje koriste standard OpenID Connect za provedbu jedinstvene prijave potražite u članku [razumijevanje jedinstvene prijave na temelju OIDC-](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)a.
- Informacije u slučaju da odaberete upisivanje koda izravnim slanjem i rukovanjem HTTP zahtjevima ili pomoću biblioteke otvorenog izvornog izvora, a ne pomoću jedne od naših otvorenih izvornih biblioteka, pročitajte članak [OAuth 2,0 i OpenID Connect protokole na Microsoftovoj platformi identiteta](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokoli**

1. [Microsoftova platforma za identifikaciju i implicitni protok potpore](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) – definiranje karakteristika implicitne potpore jest da se tokeni (ID tokeni ili token programa Access) vraćaju izravno iz krajnje točke/predautorizacije umjesto krajnje točke/tokena. To se često koristi kao dio tijeka koda za autorizaciju, u onome što se zove **"hibridni tijek" – DOHVAĆANJE ID tokena na zahtjev/autorizacija uz autorizaciju**. U ovom se članku opisuje kako programirati izravno prema protokolu u aplikaciji da biste zatražili žetone iz servisa Azure AD.
2. [Microsoftov identitet Platform i oauth 2,0 status koda za autorizaciju](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – 2,0 u aplikacijama koje su instalirane na uređaju omogućuju pristup zaštićenim resursima kao što su web-API-jevi za autorizaciju. Pomoću Microsoftove platforme za identitete sustava OAuth 2,0 možete **dodati pristup prijavi i API-ju na mobilne i aplikacije za stolna računala**. U ovom se članku opisuje kako programirati izravno prema protokolu u aplikaciji pomoću bilo kojeg jezika.
3. [Microsoftov identifikacijski okvir za identifikaciju i protokol OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) -kada koristite implementaciju OpenID-a za Microsoft Identity Platform, možete dodati pristup prijave i API-ja u aplikacije. U ovom se članku pokazuje kako to učiniti nezavisnim jezikom i opisuje kako **slati i primati HTTP poruke bez korištenja bilo koje Microsoftove biblioteke otvorenog izvora**.
4. [Microsoftova platforma za identifikaciju i tijek vjerodajnica oauth 2,0 Client](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – možete koristiti dozvolu oauth 2,0 Client vjerodajnice navedene u programu rfc 6749, ponekad se naziva i **dvosmjerna OAuth**, za pristup resursima koje hostira web-mjesto pomoću identiteta aplikacije. Ova vrsta potpore obično se koristi za interakcije poslužitelja s poslužiteljem koje se moraju pokretati u pozadini, bez neposredne interakcije s korisnikom. Te se vrste aplikacija često spominju kao **Daemoni** ili **Računi servisa**. U ovom se članku opisuje kako programirati izravno prema protokolu u aplikaciji.
