---
title: Konfiguriranje jedinstvene jedinstvene prijave (SSO)
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966029"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfiguriranje jedinstvene jedinstvene prijave (SSO)

**Konfiguriranje aplikacija**

1. Vrijednosti biste trebali dobiti od dobavljača aplikacije. Vrijednosti možete ručno unijeti ili prenijeti datoteku metapodataka da biste izdvojili vrijednost polja.
2. Mnoge su aplikacije već unaprijed konfigurirane za rad sa servisom Azure AD. Te su aplikacije navedene u galeriji aplikacija koje možete pregledavati prilikom dodavanja aplikacije na klijent azure AD. Niz [brzih početaka](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) prolazi kroz postupak.
3. Da biste stvorili aplikaciju koja nije galerija, kliknite **+ Stvori vlastitu** aplikaciju i dajte naziv aplikaciji.
    - Po zadanom će odabrati Integriraj sve **druge aplikacije** koje ne pronađete u galeriji, što je ispravna mogućnost za aplikacije koje nisu galerije.
    - Kada nakon **stavljajući** naziv aplikacije pritisnite Stvori, stvorit će se nova enterprise aplikacija koja nije galerija.
    - Zatim se možete kretati do jedinstvene  prijave **u** odjeljku Upravljanje tom aplikacijom i moći ćete vidjeti različite tehnike za implementaciju u svom okruženju.

**Konfiguriranje besprijekornog SSO-a za određenu aplikaciju**

Za aplikacije u galeriji pronaći ćete detaljne, detaljne upute. Da biste pristupili koracima, pregledajte popis svih vodiča za konfiguraciju aplikacija u vodičima za [konfiguraciju aplikacija saaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Konfiguriranje SSO-a utemeljenog na SAML-u**

1. [Brzi početak rada: postavite jedinstvenu prijavu (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)utemeljenu na SAML-u za aplikaciju u klijentu servisa Azure Active Directory (Azure AD).
2. Dodatne informacije o mogućnosti jedinstvene prijave utemeljene na SAML-u potražite u članku Razumijevanje jedinstvene prijave utemeljene na [SAML-u](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Da biste saznali više o zahtjevima za provjeru autentičnosti za SAML 2.0 i odgovorima koje Azure Active Directory (Azure AD) podržava za jednostruki Sign-On (SSO), pogledajte Sign-On [saml protokol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Da biste saznali kako stvoriti i konfigurirati jedinstvenu prijavu (SSO) utemeljenu na SAML-u za aplikaciju na servisu Azure Active Directory (Azure AD) pomoću API-ja za Microsoft Graph, pogledajte konfiguriranje jedinstvene prijave utemeljene na [SAML-u](https://docs.microsoft.com/graph/application-saml-sso-configure-api)za aplikaciju pomoću API-ja za Microsoft Graph .
5. Da biste saznali kako Azure AD koristi SAML protokol, pogledajte [kako Microsoftova platforma za identitete koristi SAML protokol](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Konfiguriranje tokena i potraživanja**

1. [Kako: prilagoditi zahtjeve izdane u SAML tokenu za korporacijske aplikacije.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Da biste saznali kako konfigurirati potraživanja pomoću komponente PowerShell, pogledajte upute: Prilagodba potraživanja emitiranih u tokenima za određenu aplikaciju [u klijentu (pretpregled).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Da biste saznali kako konfigurirati neobavezne zahtjeve, pogledajte [upute: Navedite neobavezne zahtjeve za aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Da biste saznali kako koristiti atribute proširenja sheme direktorija za slanje korisničkih podataka aplikacijama u zahtjevima za tokene, pogledajte korištenje [atributa proširenja sheme direktorija u zahtjevima](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Upute za konfiguriranje vijeka trajanja tokena pogledajte u članku Vijekovi tokena koji se mogu [konfigurirati u Microsoftova platforma za identitete (pretpregled).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Konfiguriranje pravilnika životnog ciklusa tokena (pretpregled)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – u ovom članku prolazimo kroz uobičajeni scenarij pravilnika koji vam može pomoći da nametnete nova pravila za vijek tokena. U primjeru ćete saznati kako stvoriti pravilnik za koji korisnici moraju češće provjeravati autentičnost u web-aplikaciji.

**Otklanjanje poteškoća s konfiguracijom SSO-a**

- Najčešća pitanja o jedinstvenoj jedinstvenoj Azure Active Directory (Besprijekorna jedinstvena jedinstvena Sign-On) pogledajte Azure Active Directory besprijekorna jedinstvena [prijava: najčešća pitanja](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Informacije o najčešćim problemima vezanim uz Azure Active Directory (Azure AD) Besprijekorna jedinstvena Sign-On (besprijekorna jedinstvena jedinstvena prijava) potražite u [članku Otklanjanje poteškoća Azure Active Directory besprijekornom jedinstvenom prijavom](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
