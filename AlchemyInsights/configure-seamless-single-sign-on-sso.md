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
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402259"
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

1. Brzi početak rada: postavljanje jedinstvene prijave utemeljene na [SAML-u (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)za aplikaciju na klijentu servisa Azure Active Directory (Azure AD).
2. Dodatne informacije o mogućnosti jedinstvene prijave utemeljene na SAML-u potražite u članku Razumijevanje jedinstvene prijave utemeljene na [SAML-u](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Da biste saznali više o zahtjevima za provjeru autentičnosti za SAML 2.0 i odgovorima koje Azure Active Directory (Azure AD) podržava za single Sign-On (SSO), pogledajte [jednostruki Sign-On SAML protokol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Da biste saznali kako stvoriti i konfigurirati jedinstvenu prijavu (SSO) utemeljenu na SAML-u za aplikaciju na servisu Azure Active Directory (Azure AD) pomoću API-ja za Microsoft Graph, pogledajte konfiguriranje jedinstvene prijave na SAML za aplikaciju pomoću [API-ja za Microsoft Graph](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Da biste saznali kako Azure AD koristi SAML protokol, pogledajte [kako Microsoftova platforma za identitet koristi PROTOKOL SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Konfiguriranje tokena i potraživanja**

1. [Kako: prilagoditi zahtjeve izdane u SAML tokenu za korporacijske aplikacije.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Da biste saznali kako konfigurirati potraživanja pomoću komponente PowerShell, pogledajte upute: Prilagodba potraživanja emitiranih u tokenima za određenu aplikaciju [u klijentu (pretpregled).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Da biste saznali kako konfigurirati neobavezne zahtjeve, pogledajte [upute: Navedite neobavezne zahtjeve za aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Da biste saznali kako koristiti atribute proširenja sheme direktorija za slanje korisničkih podataka aplikacijama u zahtjevima za tokene, pogledajte korištenje [atributa proširenja sheme direktorija u zahtjevima](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Da biste saznali kako konfigurirati vijek tokena, pogledajte članak Vijekovi tokena koji se mogu konfigurirati [na microsoftovoj platformi identiteta (pretpregled).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Konfiguriranje pravilnika životnog ciklusa tokena (pretpregled)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – u ovom članku prolazimo kroz uobičajeni scenarij pravilnika koji vam može pomoći da nametnete nova pravila za vijek tokena. U primjeru ćete saznati kako stvoriti pravilnik za koji korisnici moraju češće provjeravati autentičnost u web-aplikaciji.

**Otklanjanje poteškoća s konfiguracijom SSO-a**

- Najčešća pitanja o jedinstvenoj jedinstvenoj prijavi servisa Azure Active Directory Sign-On (besprijekorna jedinstvena jedinstvena prijava na [servisu Azure Active Directory): najčešća pitanja](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Informacije o otklanjanju poteškoća vezanih uz besprijekornu jedinstvenu prijavu servisa Azure Active Directory (Azure AD Sign-On) potražite u članku Otklanjanje poteškoća s jedinstvenom prijavom servisa [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
