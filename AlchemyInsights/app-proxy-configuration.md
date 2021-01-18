---
title: Konfiguracija proxyja aplikacija
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884839"
---
# <a name="app-proxy-configuration"></a>Konfiguracija proxyja aplikacija

1. Da biste razumjeli kako konfigurirati aplikaciju proxyja aplikacije u sklopu servisa Azure AD da biste u oblak izložili lokalne aplikacije, pročitajte članak [Konfiguriranje aplikacije proxyja aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Jedinstvena prijava (SSO) korisnicima omogućuje pristup aplikaciji bez provjere autentičnosti više puta. Omogućuje jedinstvenu provjeru autentičnosti u oblaku, na servisu Azure Active Directory i omogućuje oponašaju korisnika da izvrši dodatne izazove provjere autentičnosti u aplikaciji. Dodatne informacije potražite u članku [Konfiguriranje jedinstvene prijave u aplikaciju za proxy aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Pomoću [ovog članka](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) možete otkloniti česte probleme s kojima se suočavaju osobe pri stvaranju nove aplikacije za proxy aplikacije.
4. Ako imate problema s postavljanjem sigurnosne provjere autentičnosti u aplikaciji, možda ćete morati [otkloniti poteškoće s ograničenjem programa za delegiranje poslužitelja za proxy poslužitelje](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) ili pratiti upute za [Konfiguriranje aplikacije pomoću servisa pingaccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) da biste riješili problem.
