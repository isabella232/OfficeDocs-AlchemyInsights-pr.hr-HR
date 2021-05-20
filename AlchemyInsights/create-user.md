---
title: Stvaranje korisnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569703"
---
# <a name="create-user"></a><span data-ttu-id="31471-102">Stvaranje korisnika</span><span class="sxs-lookup"><span data-stu-id="31471-102">Create user</span></span>

<span data-ttu-id="31471-103">**NAJAVA:**</span><span class="sxs-lookup"><span data-stu-id="31471-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="31471-104">[Deprecation of WebView sign-in support from Google starting 4 siječnja 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span><span class="sxs-lookup"><span data-stu-id="31471-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="31471-105">Provjerite mogu li na vaše aplikacije utjecati Googleove [smjernice za](https://go.microsoft.com/fwlink/?linkid=2157323) testiranje kompatibilnosti.</span><span class="sxs-lookup"><span data-stu-id="31471-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="31471-106">Provjerite koristite li web-prikaz sustava ili preglednik sustava prilikom prijave korisnika pomoću korisničkih Google računa.</span><span class="sxs-lookup"><span data-stu-id="31471-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="31471-107">Dodatne informacije potražite u članku [Problemi prilikom prijave u aplikacije samo u pregledniku Chrome](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span><span class="sxs-lookup"><span data-stu-id="31471-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="31471-108">**Ne mogu stvoriti novog korisnika u direktoriju servisa Azure AD**</span><span class="sxs-lookup"><span data-stu-id="31471-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="31471-109">Provjerite jeste li ovlašteni za stvaranje novog standardnog korisnika.</span><span class="sxs-lookup"><span data-stu-id="31471-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="31471-110">Samo uloga globalnog administratora ili administratora korisnika u programu Azure Active Directory (AD) može stvoriti novog standardnog korisnika.</span><span class="sxs-lookup"><span data-stu-id="31471-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="31471-111">Ako niste u jednoj od tih uloga, zatražite od administratora da vas doda u jednu od tih uloga ili da vam stvori novi korisnički račun.</span><span class="sxs-lookup"><span data-stu-id="31471-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="31471-112">Provjerite nalazi li se korisničko ime u domeni potvrđenoj u servisu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="31471-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="31471-113">Ako na servisu Azure AD nema potvrđenih prilagođenih naziva domena, možete koristiti početnu domenu servisa Azure AD, koja završava s \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="31471-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="31471-114">Provjerite je li korisničko ime u domeni koja nije pridružena servisu Azure AD iz lokalnog AD-a.</span><span class="sxs-lookup"><span data-stu-id="31471-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="31471-115">Korisnike nije moguće dodati u oblak s nazivima domena koji su pridruženi lokalno.</span><span class="sxs-lookup"><span data-stu-id="31471-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="31471-116">Provjerite ima li nijedan drugi korisnik ili kontakt korisničko ime koje želite dodijeliti novom korisniku.</span><span class="sxs-lookup"><span data-stu-id="31471-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="31471-117">Korisnička imena moraju biti jedinstvena na servisu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="31471-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="31471-118">Pogledajte [uloge i administratore servisa Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="31471-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="31471-119">Pogledajte [nazive domena za](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="31471-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="31471-120">Pregledajte [zapisnike nadzora](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) da biste vidjeli detaljnije informacije o nedavno stvorenom ili izbrisanom korisniku, npr. o tome tko je izveo akciju i kada.</span><span class="sxs-lookup"><span data-stu-id="31471-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="31471-121">Dodatne informacije o dodavanju novih korisnika potražite u članku Stvaranje novog korisnika na [servisu Azure AD](/azure/active-directory/active-directory-users-create-azure-portal)pomoću portala Azure .</span><span class="sxs-lookup"><span data-stu-id="31471-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="31471-122">[Administratorske uloge servisa Azure AD](/azure/active-directory/active-directory-assign-admin-roles): administratorske dozvole za Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="31471-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="31471-123">Da biste stvorili [novog korisnika, možete koristiti](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)i Azure AD PowerShell .</span><span class="sxs-lookup"><span data-stu-id="31471-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
