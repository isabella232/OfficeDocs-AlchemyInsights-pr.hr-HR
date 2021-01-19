---
title: Otklanjanje poteškoća s korisnikom gosta
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900832"
---
# <a name="troubleshoot-guest-user-issues"></a>Otklanjanje poteškoća s korisnikom gosta

1. Upute za upravljanje pristupom gosta aplikacijama potražite u članku [Upravljanje pristupom gostu uz recenzije servisa Azure ad Access](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Dodajte goste u svoj direktorij na portalu Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): u ovom ćete Quickstart dodati novog gosta u direktorij Azure ad putem portala Azure, poslat ćete pozivnicu i vidjeti kako izgleda postupak otkupljenja poziva korisnika.
1. [Dodajte korisnika gosta pomoću komponente PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): u ovom ćete Quickstart koristiti naredbu New-AzureADMSInvitation da biste jedan gost korisnika dodali svom klijentu za Azure.
1. Upute za dodjelu korisnika i grupa u Enterprise aplikacije u servisu Azure Active Directory (Azure AD) na portalu Azure ili pomoću komponente PowerShell potražite [u članku Upravljanje korisničkim zadatkom za aplikaciju u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. B2B suradnja u servisu Azure Active Directory (Azure AD) funkcionira s većini aplikacija koje se integriraju s Azure AD. U ovom ćemo [članku](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)proći kroz upute za konfiguriranje nekih popularnih aplikacija SaaS za korištenje s programom Azure ad B2B.
1. Kao tvrtka ili ustanova koja koristi značajke B2B suradnje servisa Azure Active Directory (Azure AD) da biste korisnicima korisnika pozvali iz partnerskih organizacija na Azure AD, sada možete ovim B2B korisnicima pružiti pristup lokalnim aplikacijama. Te lokalne aplikacije mogu koristiti provjeru autentičnosti utemeljenu na SAML-u ili integriranu provjeru autentičnosti sustava Windows (IWA) uz Kerberos ograničeno delegiranje (KCD). Dodatne informacije potražite u članku [Dodjela B2B korisnika u aplikaciji Azure ad za pristup lokalnim aplikacijama](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Informirajte se o tome kako [dodijeliti lokalno upravljanim partnerom računima pristup resursima u oblaku pomoću suradnje Azure ad B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).