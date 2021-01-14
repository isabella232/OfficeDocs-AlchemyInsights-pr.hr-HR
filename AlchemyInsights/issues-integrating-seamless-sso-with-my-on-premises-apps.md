---
title: Problemi s integriranjem bešavnih SSO-a s lokalnim aplikacijama
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868651"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemi s integriranjem bešavnih SSO-a s lokalnim aplikacijama

Da biste otklonili poteškoće s integriranjem besprijekornog SSO-a s lokalnim aplikacijama, učinite sljedeće:

**Preporučeni koraci**

1. Da biste konfigurirali **lokalnu aplikaciju** za **jedinstvenu prijavu putem proxyja aplikacija**, pročitajte članak [issvođivanje lozinki za jedinstvenu prijavu uz proxy aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Otklanjanje poteškoća s proxyjem aplikacija**: preporučujemo da počnete s pregledom tijeka rada za otklanjanje poteškoća, otklanjanjem [problema s proxyjem aplikacija](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), da biste odredili jesu li poveznici za proxy aplikacije pravilno konfigurirani. Ako i dalje imate problema s povezivanjem s aplikacijom, slijedite korake za otklanjanje poteškoća u odjeljku [ispravljanje problema s aplikacijom proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)aplikacija. Probleme s [CORS možete identificirati](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) pomoću sljedećih alata za ispravljanje pogrešaka u pregledniku:
    1. Pokrenite preglednik i potražite web-aplikaciju.
    1. Pritišćite **F12** da biste postavili konzolu za ispravljanje pogrešaka.
    1. Pokušajte reproducirati transakciju i pregledajte poruku konzole. Kršenje CORS-a stvara pogrešku konzole o porijeklu.
    1. Neki problemi sa vezom ne mogu se razriješiti, kao što je kada aplikacija preusmjerava na login.microsoftonline.com u provjeru autentičnosti i istekne token programa Access. Kada se CORS nazove, neće uspjeti. Zaobilazno rješenje za ovaj scenarij jest produžiti vijek trajanja tokena programa Access da bi se spriječilo da istječe tijekom korisničke sesije. Dodatne informacije o tome kako to učiniti potražite u članku [konfiguriranja načina trajanja tokena u Microsoftovoj platformi Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Preporučeni dokumenti**

- [Konfiguriranje jedinstvene prijave u aplikacijsku aplikaciju za proxy aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Single prijava za lokalne aplikacije s aplikacijom proxy poslužitelja](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Razumijevanje i rješavanje problema s proxyjem aplikacije Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Otklanjanje poteškoća s ograničenim konfiguracijama delegacije za proxy poslužitelje programa Kerberos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)