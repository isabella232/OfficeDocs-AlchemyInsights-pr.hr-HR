---
title: Otklanjanje poteškoća s besprijekornom jedinstvenom prijavom (SSO- om) utemeljenim na lozinki
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
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972816"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Otklanjanje poteškoća s besprijekornom jedinstvenom prijavom (SSO- om) utemeljenim na lozinki

Informacije o osnovama SSO-a utemeljenog na lozinki pogledajte u članku [Provjera autentičnosti utemeljena](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)na lozinki Azure Active Directory .

**Konfiguriranje SSO-a utemeljenog na lozinki**

1. [Konfiguriranje jedinstvene prijave utemeljene na lozinki](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – u ovom se članku detaljnije govori o mogućnosti jedinstvene prijave utemeljene na lozinki. Ako aplikacija koju dodajete zahtijeva prilagođenu konfiguraciju i morate koristiti SSO utemeljen na lozinki, ovaj je članak za vas.
2. [Konfigurirajte jedinstvenu prijavu utemeljenu](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) na lozinki za pret-aplikacije – proxy aplikacije podržava nekoliko načina jedinstvene prijave. Prijava utemeljena na lozinki namijenjena je aplikacijama koje koriste kombinaciju korisničkog imena i lozinke za provjeru autentičnosti. Kada konfigurirate prijavu utemeljenu na lozinki za aplikaciju, korisnici se moraju prijaviti u lokalnu aplikaciju jednom. Nakon toga Azure Active Directory podatke za prijavu i automatski ih pruža aplikaciji kada korisnici pristupaju daljinski.
    - Aplikaciju ste već trebali objaviti i testirati pomoću proxyja aplikacije. Ako ne, slijedite korake u nastavku Objavljivanje aplikacija pomoću proxyja [aplikacije Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) a zatim nastavite s konfiguracijom SSO-a utemeljenog na lozinki za aplikacije na premu.

Da biste otklonili poteškoće s jedinstvenom prijavom utemeljenom na lozinki, pogledajte otklanjanje poteškoća s [jedinstvenom prijavom na azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
