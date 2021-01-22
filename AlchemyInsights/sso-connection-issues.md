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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935087"
---
# <a name="sso-connection-issues"></a>Problemi s vezom za SSO

1. Slijedite gumb [Quickstart: konfigurirajte svojstva za vodič aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) da biste konfigurirali aplikaciju.
2. Ovisno o odabranoj mogućnosti aplikacije i [jedinstvene prijave](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) , slijedite odgovarajuće smjernice u nastavku:
    - Da biste konfigurirali **lokalnu aplikaciju** za **jedinstvenu prijavu sa sjedištem u saml-** u, pročitajte članak [saml koji se prijavljuje za lokalne aplikacije uz proxy aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Da biste konfigurirali **aplikaciju u oblaku** za **jedinstvenu prijavu utemeljenu na lozinci**, pročitajte članak  [Konfiguriranje jedinstvene prijave za lozinku](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Da biste konfigurirali **lokalnu aplikaciju** za **jedinstvenu prijavu putem proxyja aplikacija**, pročitajte članak [issvođivanje lozinki za jedinstvenu prijavu uz proxy aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Otklanjanje poteškoća s proxyjem aplikacija**: preporučujemo da počnete s pregledom tijeka rada za otklanjanje poteškoća, otklanjanjem [problema s proxyjem aplikacija](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), da biste odredili jesu li poveznici za proxy aplikacije pravilno konfigurirani. Ako i dalje imate problema s povezivanjem s aplikacijom, pratite tijek otklanjanja poteškoća u [problemima s aplikacijom proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)aplikacije za ispravljanje pogrešaka. Probleme s [CORS možete identificirati](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) pomoću alata za ispravljanje pogrešaka u pregledniku:
    - Pokrenite preglednik i potražite web-aplikaciju.
    - Pritišćite **F12** da biste postavili konzolu za ispravljanje pogrešaka.
    - Pokušajte reproducirati transakciju i pregledajte poruku konzole. Kršenje CORS-a stvara pogrešku konzole o porijeklu.
    - Neki problemi sa vezom ne mogu se razriješiti, kao što je kada aplikacija preusmjerava na login.microsoft.com u provjeru autentičnosti i istekne token programa Access. Kada se CORS nazove, neće uspjeti. Zaobilazno rješenje za ovaj scenarij jest produžiti vijek trajanja tokena programa Access da bi se spriječilo da istječe tijekom korisničke sesije. Dodatne informacije o tome kako to učiniti potražite u članku [konfiguriranja načina trajanja tokena u Microsoftovoj platformi Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Otklanjanje poteškoća s jedinstvenom prijavom na saml**: preporučujemo provjeru [problema prilikom prijave u pojedinačne aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)koje se temelje na jednom servisu, da biste pronašli rješenja za probleme s kojima ćete najvjerojatnije naići.
5. **Otklanjanje poteškoća s jedinstvenom prijavom na lozinku**: preporučujemo da na servisu [Azure ad pronađete otklanjanje poteškoća s jedinstvenom prijavom na lozinku](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), da biste pronašli rješenja problema na koje najvjerojatnije nailazite.
6. Problemi s povezivanjem tijekom korištenja VPN-a potražite [u članku Korištenje jedinstvene prijave (SSO) putem VPN-a i Wi-Fi veza](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
