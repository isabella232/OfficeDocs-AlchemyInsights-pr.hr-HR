---
title: Konfiguriranje neprekinutu jedinstvenu prijavu (SSO)
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
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841420"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfiguriranje neprekinutu jedinstvenu prijavu (SSO)

**Konfiguriranje aplikacija**

1. Vrijednosti možete nabaviti od dobavljača aplikacije. Možete ručno unijeti vrijednosti ili prenijeti datoteku metapodataka da biste izdvojili vrijednost polja.
2. Mnoge su aplikacije već konfigurirane za rad s Azure AD-om. Te su aplikacije navedene u galeriji aplikacija koje možete pregledavati prilikom dodavanja aplikacije u klijent za Azure AD. [Serija programa Quickstart](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) prolazi kroz postupak.
3. Da biste stvorili aplikaciju koja nije galerija, možete kliknuti na **+ stvoriti vlastiti gumb aplikacija** i dati naziv aplikaciji.
    - Po zadanom će odabrati **integraciju bilo koje druge aplikacije koju ne pronađete u galeriji** koja je ispravna mogućnost za aplikacije koje nisu u galeriji.
    - Kada kliknete **Stvori** nakon stavljanja naziva za aplikaciju, stvorit će novu korporacijsku aplikaciju koja se ne nalazi u galeriji.
    - Zatim možete prijeći na **jedinstvenu prijavu** u odjeljku **Upravljanje** tom aplikacijom i moći ćete vidjeti razne tehnike za njihovo implementaciju u svom okruženju.

**Konfiguriranje bešavnih SSO-a za određenu aplikaciju**

Za aplikacije u galeriji prikazat će se Detaljne, detaljne upute. Da biste pristupili koracima, možete pregledavati popis svih vodiča za konfiguriranje aplikacija na [tutorijalima za konfiguriranje aplikacija SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Konfiguracija komponente sa sjedištem u SAML-u**

1. Brzi [početak rada: postavite jedinstvenu prijavu za SAML (SSO) za aplikaciju u klijentu Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Dodatne informacije o mogućnostima utemeljenoj na SAML-u potražite u članku [razumijevanje jedinstvene prijave na temelju saml-](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)a.
3. Da biste saznali više o zahtjevima za provjeru autentičnosti SAML 2,0 i odgovorima koje podržava Azure Active Directory (Azure AD) za single Sign-On (SSO), pročitajte članak [Single Sign-On za saml protokol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Da biste doznali kako stvoriti i konfigurirati jedinstvenu prijavu (SSO) u sustavu Azure Active Directory (Azure AD) pomoću API-ja programa Microsoft Graph, pročitajte članak [Konfiguriranje jedinstvene prijave na temelju SAML-a za svoju aplikaciju pomoću API-ja za Microsoft Graph](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Da biste doznali kako Azure AD koristi protokol SAML, pročitajte članak [Kako Microsoftova platforma za identitete koristi saml protokol](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Konfiguriranje tokena i potraživanja**

1. [Kako: prilagoditi potraživanja izdane u programu SAML token za Enterprise Applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Da biste doznali kako konfigurirati zahtjeve pomoću komponente PowerShell, pročitajte članak [Kako: prilagoditi tvrdnje koje se emitiraju u tokena za određenu aplikaciju u klijentu (pretpregled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Upute za konfiguriranje neobaveznih potraživanja potražite u članku [upute za pružanje neobaveznih zahtjeva za aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Upute za korištenje atributa proširenja sheme direktorija za slanje korisničkih podataka u aplikacije u tvrdnjama tokena potražite [u članku Korištenje atributa proširenja sheme direktorija u tvrdnjama](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Da biste doznali kako konfigurisati životni vijek tokena, pročitajte članak [sažima tokena životni vijek u Microsoftovoj platformi Identity (pretpregled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Konfiguriranje pravila životnog vijeka tokena (pretpregled)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – u ovom ćemo članku proći kroz uobičajen scenarij pravilnika koji će vam pomoći u nametanju novih pravila za vijek trajanja tokena. U primjeru ćete naučiti kako stvoriti pravilo za koje korisnici moraju češće provjeravati autentičnost u web-aplikaciji.

**Otklanjanje poteškoća s konfiguracijom SSO**

- Najčešća pitanja vezana uz neprekinutu jedinstvenu Sign-On (bešavni SSO) u članku [Azure Active Directory neprekinutu jedinstvenu prijavu: najčešća pitanja](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Informacije o otklanjanju poteškoća s uobičajenim problemima vezanih uz Azure Active Directory (Azure AD) bez neprekinutih pojedinačnih Sign-On (besprijekoran SSO) potražite u članku [Otklanjanje poteškoća s jedinstvenim prijavom u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
