---
title: Problemi s vezom za SSO
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
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084338"
---
# <a name="sso-connection-issues"></a>Problemi s vezom za SSO

1. Slijedite [brzi početak rada: konfigurirajte svojstva vodiča za aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) da biste konfigurirali aplikaciju.
2. Ovisno o odabranoj aplikaciji [i mogućnosti jedinstvene prijave,](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) slijedite odgovarajuće smjernice u nastavku:
    - Da biste **konfigurirali lokalnu** aplikaciju za jedinstvenu prijavu utemeljenu na **SAML-u**, pogledajte SAML jedinstvenu prijavu za lokalne aplikacije [s proxyjem aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Da biste **konfigurirali aplikaciju u oblaku** **za jedinstvenu prijavu** utemeljenu na lozinki , pogledajte konfiguriranje jedinstvene prijave  [lozinkom](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Da biste **konfigurirali lokalnu aplikaciju** za jedinstvenu prijavu putem **proxyja aplikacije**, pogledajte sefing lozinke za [jedinstvenu prijavu pomoću proxyja aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Otklanjanje poteškoća s proxyjem** aplikacije : preporučujemo da počnete s pregledom tijeka otklanjanja poteškoća, problema s [debugiranjem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)proxy poveznika aplikacije da biste utvrdili jesu li konektori proxyja aplikacije pravilno konfigurirani. Ako i dalje imate problema s povezivanjem s aplikacijom, slijedite tijek otklanjanja poteškoća u problemima s aplikacijom [Proxy aplikacije za ispravljanje pogrešaka.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Pomoću alata [za ispravljanje pogrešaka u pregledniku](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) možete prepoznati probleme s alatima za ispravljanje pogrešaka u pregledniku:
    - Pokrenite preglednik i dođite do web-aplikacije.
    - Pritisnite **F12 da biste** smislili konzolu za ispravljanje pogrešaka.
    - Pokušajte reproducirati transakciju i pregledati poruku konzole. Zbog kršenja pravila o KORS-u došlo je do pogreške konzole u vezi s ishodištem.
    - Neke probleme s CORS-om nije moguće riješiti, primjerice kada se aplikacija preusmjeri na login.microsoft.com provjeru autentičnosti, a token za pristup istekne. Poziv za CORS tada ne uspijeva. Zaobilazno rješenje za taj scenarij jest produljiti vijek trajanja pristupnog tokena da biste spriječili da istječe tijekom korisnikova sesije. Dodatne informacije o tome kako to učiniti potražite u članku Vijekovi [tokena](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)koji se mogu konfigurirati Microsoftova platforma za identitete .
4. Otklanjanje poteškoća s jedinstvenom prijavom utemeljenom na **SAML-u**: preporučujemo da provjerite probleme prilikom prijave u konfigurirane aplikacije utemeljene na [SAML-u](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)da biste pronašli rješenja za probleme na koje ćete najvjerojatnije naići.
5. **Otklanjanje poteškoća s jedinstvenom** prijavom na temelju lozinke : preporučujemo da provjerite otklanjanje poteškoća s jedinstvenom prijavom na [servisu Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)utemeljenom na lozinki da biste pronašli rješenja za probleme na koje najčešće nailazite.
6. Probleme s povezivanjem tijekom korištenja VPN-a pogledajte u članku Korištenje jedinstvene prijave [(SSO) putem VPN-a i Wi-Fi veza](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
