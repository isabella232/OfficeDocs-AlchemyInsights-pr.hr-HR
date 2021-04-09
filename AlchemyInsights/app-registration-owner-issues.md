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
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404293"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="7149b-102">Problemi s vlasnikom registracije aplikacije</span><span class="sxs-lookup"><span data-stu-id="7149b-102">App Registration Owner issues</span></span>

<span data-ttu-id="7149b-103">Slijede dostupni načini dodavanja upravitelja kao vlasnika za registracije aplikacija:</span><span class="sxs-lookup"><span data-stu-id="7149b-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="7149b-104">Korištenje modula Azure AD PowerShell –</span><span class="sxs-lookup"><span data-stu-id="7149b-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="7149b-105">Referenca: [Add-AzureAdApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="7149b-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="7149b-106">Korištenje platforme Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="7149b-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="7149b-107">Referenca: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="7149b-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="7149b-108">Korištenje ms graph -</span><span class="sxs-lookup"><span data-stu-id="7149b-108">Using MS Graph -</span></span>

    <span data-ttu-id="7149b-109">Referenca: [Dodavanje vlasnika – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="7149b-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="7149b-110">Korištenje portala Azure AD – idite [na portal.azure.com](https://portal.azure.com/) > Azure Active directory > Registracija aplikacije > Odaberite aplikaciju > Vlasnici > Dodaj vlasnike</span><span class="sxs-lookup"><span data-stu-id="7149b-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="7149b-111">**Nije moguće prikazati aplikaciju na oštrici Registracije aplikacija iako ste vlasnik te aplikacije?**</span><span class="sxs-lookup"><span data-stu-id="7149b-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="7149b-112">Vlasnik aplikacije nije administrativna uloga.</span><span class="sxs-lookup"><span data-stu-id="7149b-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="7149b-113">Ako je [omogućena postavka Ograniči pristup portalu za](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) administraciju servisa Azure AD, samo administrator moći će pregledavati aplikacije na portalu za registraciju aplikacija.</span><span class="sxs-lookup"><span data-stu-id="7149b-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="7149b-114">Da bi vlasnik mogao pregledavati aplikacije, onemogućite tu postavku (Postavite tu postavku na NE) ili dodijelite administratorsku ulogu vlasniku samo za određenu aplikaciju.</span><span class="sxs-lookup"><span data-stu-id="7149b-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="7149b-115">No za to će vam biti potrebna licenca za Azure AD Premium P2 i omogućivanje upravljanja [privilegiranim identitetom.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="7149b-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>