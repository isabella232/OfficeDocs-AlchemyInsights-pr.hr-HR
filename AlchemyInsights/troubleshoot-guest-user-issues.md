---
title: Otklanjanje poteškoća s gostom
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939371"
---
# <a name="troubleshoot-guest-user-issues"></a>Otklanjanje poteškoća s gostom

1. Smjernice o upravljanju pristupom gosta aplikacijama pogledajte u članku [Upravljanje pristupom gosta uz preglede pristupa servisa Azure AD](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. Dodavanje gostiju u direktorij na [portalu Azure:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)u ovom brzom vodiču dodat ćete novog gosta u direktorij servisa Azure AD putem portala Azure, poslati pozivnicu i vidjeti kako izgleda postupak otkupa pozivnice gosta.
1. [Dodajte gosta pomoću komponente PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)u ovom brzom počnite koristiti naredbu New-AzureADMSInvitation da biste dodali jednog gosta na klijent servisa Azure.
1. Da biste saznali kako korisnicima i grupama dodijeliti korporacijske aplikacije na servisu Azure Active Directory (Azure AD), bilo s portala Azure ili pomoću komponente PowerShell, pogledajte upravljanje korisničkim zadacima [za aplikaciju u sustavu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B suradnja funkcionira s većinom aplikacija koje se integriraju sa servisom Azure AD. U ovom članku pročešijamo upute za konfiguriranje nekih popularnih aplikacija saaS za korištenje sa servisom Azure AD B2B. [](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)
1. Kao tvrtka ili ustanova koja koristi Azure Active Directory (Azure AD) B2B mogućnosti suradnje za pozivanje gostiju iz partnerskih tvrtki ili ustanova na Azure AD, sada tim B2B korisnicima možete omogućiti pristup lokalnim aplikacijama. Te lokalne aplikacije mogu koristiti provjeru autentičnosti utemeljenu na SAML-u ili integriranu provjeru autentičnosti Windows (IWA) uz kerberos ograničeno delegiranje (KCD). Dodatne informacije potražite u članku [Dodjela B2B korisnicima na servisu Azure AD pristup](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)lokalnim aplikacijama .
1. Saznajte kako lokalnim partnerskim računima dodijeliti pristup resursima u [oblaku pomoću suradnje na servisu Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).