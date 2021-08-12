---
title: Problemi s vlasnikom registracije aplikacije
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
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951125"
---
# <a name="app-registration-owner-issues"></a>Problemi s vlasnikom registracije aplikacije

Slijede dostupni načini dodavanja upravitelja kao vlasnika za registracije aplikacija:

- Korištenje modula Azure AD PowerShell –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referenca: [Add-AzureAdApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Korištenje platforme Azure CLI - `az ad app owner add`

    Referenca: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Korištenje ms Graph -

    Referenca: [Dodavanje vlasnika – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Korištenje portala Azure AD – idite [na portal.azure.com](https://portal.azure.com/) > Azure Active directory > Registracija aplikacije > Odaberite aplikaciju > Vlasnici > Dodaj vlasnike

**Nije moguće prikazati aplikaciju na oštrici Registracije aplikacija iako ste vlasnik te aplikacije?**

Vlasnik aplikacije nije administrativna uloga. Ako je [omogućena postavka Ograniči pristup portalu za](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) administraciju servisa Azure AD, samo administrator moći će pregledavati aplikacije na portalu za registraciju aplikacija. Da bi vlasnik mogao pregledavati aplikacije, onemogućite tu postavku (Postavite tu postavku na NE) ili dodijelite administratorsku ulogu vlasniku samo za određenu aplikaciju. No za to će vam biti potrebna licenca za Azure AD premium P2 i [omogućivanje Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
