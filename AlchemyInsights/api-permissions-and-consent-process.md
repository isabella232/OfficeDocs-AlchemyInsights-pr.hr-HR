---
title: Api Dozvole i proces pristanka
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
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932053"
---
# <a name="api-permissions-and-consent-process"></a>Api Dozvole i proces pristanka

Da bi vaša aplikacija pristupala podacima u aplikaciji Microsoft Graph, korisnik ili administrator moraju mu dodijeliti odgovarajuće dozvole putem postupka pristanka. [Referenca Graph dozvola tvrtke Microsoft](https://docs.microsoft.com/graph/permissions-reference) navodi dozvole povezane sa svakim glavnim skupom API-ja Graph Microsofta. Sadrži i smjernice za korištenje dozvola.

**Postavljanje ili ažuriranje upravitelja servisa**

- [Stvaranje servisaprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – u ovom se članku prikazuje stvaranje novog objekta servisaPrincipal.
- [Stvaranje upravitelja servisa Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) na portalu – u ovom se članku prikazuje kako stvoriti novu aplikaciju Azure Active Directory (Azure AD) i upravitelja servisa koji se mogu koristiti s kontrolom pristupa utemeljenom na ulogama.
- [Aplikacije & upravitelji](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) servisa na servisu Azure AD – u ovom se članku opisuju registracija aplikacija, objekti aplikacije i upravitelji servisa u sustavu Azure Active Directory: što su, kako se koriste i kako su međusobno povezani.

**Dodavanje i ažuriranje registracije aplikacije te pristanak administratora**

- [Stvaranje registracije aplikacije](https://docs.microsoft.com/graph/api/application-post-applications) – u ovom se članku prikazuje kako stvoriti novi objekt aplikacije.
- [Ažuriranje registracije aplikacije – dozvole za API](https://docs.microsoft.com/graph/api/application-update) – u ovom se članku pokazuje kako ažurirati svojstva objekta aplikacije.
- [Dajte pristanak administratora](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – za pristanak i pristanak administratora općenito, od administratora zahtijevamo da izričito odobri pristanak.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – spremnik za upravljanje ulogama za definicije objedinjenih uloga i zadatke uloga za davatelje Microsoft 365 RBAC koji podržavaju više upravitelja i višestruke opsege u jednom zadatku uloge. To se razlikuje od *vrste resursa rbacApplication.* Microsoft Intune primjer je takvog davatelja usluge RBAC- a. Zadatak uloge u programu Intune može imati polje upravitelja i polje grupa opsega. **To je beta verzija, što znači da je još u razvoju i ne preporučuje se za korištenje u proizvodnji.**
