---
title: Konfiguracija proxyja aplikacije
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
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951557"
---
# <a name="app-proxy-configuration"></a>Konfiguracija proxyja aplikacije

1. Upute za konfiguriranje aplikacije proxy aplikacije na servisu Azure AD da biste lokalne aplikacije izložili oblaku, pogledajte upute za konfiguriranje [aplikacije Proxy aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Jedinstvena prijava (SSO) korisnicima omogućuje pristup aplikaciji bez višestruke provjere autentičnosti. Omogućuje da se jedinstvena provjera autentičnosti odvija u oblaku, Azure Active Directory i omogućuje servisu ili povezniku da oponaša korisnika da dovrši dodatne izazove provjere autentičnosti iz aplikacije. Dodatne informacije potražite u članku Konfiguriranje jedinstvene prijave u aplikaciju [Proxy aplikacije aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Pomoću [ovog članka otklanjajte](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) poteškoće s kojima se osobe suočavaju prilikom stvaranja nove aplikacije proxy aplikacije.
4. Ako imate problema s postavljanjem zamjenske provjere autentičnosti u aplikaciji, možda ćete morati otkloniti poteškoće s [konfiguracijom kerberos ograničenog](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) delegiranja za proxy aplikacije ili slijediti smjernice o konfiguriranju aplikacije pomoću značajke [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) da biste riješili problem.
