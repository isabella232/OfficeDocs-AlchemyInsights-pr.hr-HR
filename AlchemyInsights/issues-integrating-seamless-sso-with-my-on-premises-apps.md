---
title: Problemi s integriranjem besprijekornog SSO-a s lokalnim aplikacijama
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028284"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemi s integriranjem besprijekornog SSO-a s lokalnim aplikacijama

Da biste otklonili poteškoće s integriranjem besprijekornog SSO-a s lokalnim aplikacijama, učinite sljedeće:

**Preporučeni koraci**

1. Da biste **konfigurirali lokalnu aplikaciju** za jedinstvenu prijavu putem **proxyja aplikacije**, pogledajte sefing lozinke za [jedinstvenu prijavu pomoću proxyja aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Otklanjanje poteškoća s proxyjem** aplikacije : preporučujemo da počnete s pregledom tijeka otklanjanja poteškoća, problema s [debugiranjem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)proxy poveznika aplikacije da biste utvrdili jesu li konektori proxyja aplikacije pravilno konfigurirani. Ako i dalje imate problema s povezivanjem s aplikacijom, slijedite korake za otklanjanje poteškoća u problemima s [proxyjem aplikacije za ispravljanje pogrešaka.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Probleme s [corsom možete prepoznati](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) pomoću sljedećih alata za ispravljanje pogrešaka u pregledniku:
    1. Pokrenite preglednik i dođite do web-aplikacije.
    1. Pritisnite **F12 da biste** smislili konzolu za ispravljanje pogrešaka.
    1. Pokušajte reproducirati transakciju i pregledati poruku konzole. Zbog kršenja pravila o KORS-u došlo je do pogreške konzole u vezi s ishodištem.
    1. Neke probleme s CORS-om nije moguće riješiti, primjerice kada se aplikacija preusmjeri na login.microsoftonline.com provjeru autentičnosti, a token za pristup istekne. Poziv za CORS tada ne uspijeva. Zaobilazno rješenje za taj scenarij jest produljiti vijek trajanja pristupnog tokena da biste spriječili da istječe tijekom korisnikova sesije. Dodatne informacije o tome kako to učiniti potražite u članku Vijekovi [tokena](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)koji se mogu konfigurirati Microsoftova platforma za identitete .

**Preporučeni dokumenti**

- [Konfiguriranje jedinstvene prijave u aplikaciju Proxy aplikacije aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML jedinstvena prijava za lokalne aplikacije s proxyjem aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Razumijevanje i rješavanje Azure Active Directory problema s proxyjem aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Otklanjanje poteškoća s konfiguracijom ograničenog delegiranja sustava Kerberos za proxy aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)