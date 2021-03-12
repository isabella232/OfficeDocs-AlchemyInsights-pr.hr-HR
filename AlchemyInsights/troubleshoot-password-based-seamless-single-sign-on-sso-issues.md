---
title: Otklanjanje poteškoća s jedinstvenom prijavom (SSO) koje se temelje na lozinkama
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
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714678"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Otklanjanje poteškoća s jedinstvenom prijavom (SSO) koje se temelje na lozinkama

Da biste naučili osnove dodatka SSO, pročitajte članak [Provjera autentičnosti temeljena na lozinkama pomoću servisa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Konfigurirajte SSO utemeljenu na lozinci**

1. [Konfigurirajte jedinstvenu prijavu utemeljenu na lozinci](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) u ovom članku prikazuje se detaljnije o mogućnosti SSO koje se temelje na lozinkama. Ako aplikacija koju dodajete zahtijeva prilagođenu konfiguraciju i morate koristiti SSO na temelju lozinke, ovaj je članak namijenjen vama.
2. [Konfigurirajte jedinstvenu prijavu utemeljenu na lozinkama za aplikacije na – Prem Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) -Application proksiji podržava nekoliko pojedinačnih načina prijave. Prijava temeljena na lozinkama namijenjena je aplikacijama koje koriste kombinaciju korisničkog imena i lozinke za provjeru autentičnosti. Kada konfigurirate prijavu utemeljenu na lozinci za aplikaciju, korisnici se moraju prijaviti u lokalnu aplikaciju jednom. Nakon toga, Azure Active Directory pohranjuje podatke za prijavu i automatski ga pruža aplikaciji kada korisnici na daljinu pristupe.
    - Već ste trebali objaviti i testirati aplikaciju uz proxy aplikacije. Ako ne, slijedite korake u članku [Objava aplikacija pomoću proxy poslužitelja Azure ad Application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , a zatim nastavite s konfiguracijom SSO-a utemeljenih na lozinkama za aplikacije u programu on-Prem.

Da biste otklonili problem sa SSO-om, pročitajte članak [Otklanjanje poteškoća s jedinstvenom prijavom u Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
