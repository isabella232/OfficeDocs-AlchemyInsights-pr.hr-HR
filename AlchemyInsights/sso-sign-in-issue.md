---
title: Neprimjetni problemi s prijavom u SSO
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
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935093"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Neprimjetni problemi s prijavom u SSO

Kada korisnik potvrdi autentičnost, preglednik će predmemorirati korisničke vjerodajnice da bi se u istom pregledniku aplikacija automatski prijavila s istim računom. To može otežati drugom korisniku ili jednom korisniku da se prijavljuje na više računa na jednom uređaju. Da biste riješili ovaj: 1. Pokušajte se prijaviti u neki drugi preglednik. 2. Poništite predmemoriranje i/ili kolačiće preglednika, a zatim se pokušajte ponovno prijaviti.

Ako i dalje nailazite na probleme s prijavom, preporučujemo sljedeće da dijagnosticirajte i automatizirati korake sanacije:

1. Instalirajte [proširenje preglednika moje aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) da biste pomogli servisu Azure Active Directory (Azure AD) da osiguraju bolju dijagnozu i rezolucije prilikom korištenja iskustva s testiranjem na portalu Azure.
2. Reproducirat će se pogreška pomoću iskustva testiranja na stranici za konfiguraciju aplikacija na portalu Azure. Dodatne informacije potražite u članku [Primjena pojedinačnih prijava u programu debug SAML](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Ako koristite iskustvo testiranja na portalu Azure uz proširenje preglednika moje aplikacije, možete **preskočiti četvrti korak**.
4. Da biste otvorili stranicu s jedinstvenom prijavom na SAML-u:
    - Otvorite [portal Azure](https://portal.azure.com/) i prijavite se kao **globalni administrator** ili **koadministrator**.
    - Otvorite **datotečni nastavak Azure Active Directory** tako da odaberete **sve servise** pri vrhu glavnog navigacijskih izbornika na lijevoj strani.
    - U okvir za pretraživanje filtra upišite "Azure Active Directory" i odaberite stavku **Azure Active Directory** .
    - Odaberite **Enterprise Applications** iz navigacijskog izbornika Azure Active Directory na lijevoj strani.
    - Odaberite **sve aplikacije** da biste prikazali popis svih aplikacija. Ako ne vidite aplikaciju koju želite ovdje prikazati, pomoću kontrole **filtriranja** pri vrhu **popisa sve aplikacije** postavite mogućnost **Prikaži** na **sve aplikacije**.
    - Odaberite aplikaciju koju želite konfigurirati za jedinstvenu prijavu.
    - Kada se aplikacija učitava, odaberite **jedinstvenu prijavu** na navigacijskom izborniku aplikacije na lijevoj strani.
    - Kliknite **SSO na temelju saml-** a.
5. Na temelju pogreške Saznajte više o preporučenim koracima koje treba slijediti potražite [u članku problemi prilikom prijave na pojedinačne aplikacije koje se temelje na jednom prijavom na SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. Da biste otklonili poteškoće s drugim korisničkim znakovima, obratite se sljedećim smjernicama:
    - [Single Sign-On SAML protokol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Otklanjanje poteškoća s prijavom pomoću izvješća servisa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Neočekivan upit za pristanak](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Pogreška korisničkog pristanka](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problemi s prijavom iz mojih aplikacija](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Pogreška na stranici za prijavu u aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problem prilikom prijave u Microsoftovu aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
