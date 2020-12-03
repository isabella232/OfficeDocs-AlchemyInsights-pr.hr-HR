---
title: Brisanje korisnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564419"
---
# <a name="delete-tenant"></a><span data-ttu-id="b416c-102">Brisanje korisnika</span><span class="sxs-lookup"><span data-stu-id="b416c-102">Delete tenant</span></span>

<span data-ttu-id="b416c-103">Da biste izbrisali Azure AD, provjerite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="b416c-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="b416c-104">Vi ste globalni administrator u direktoriju.</span><span class="sxs-lookup"><span data-stu-id="b416c-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="b416c-105">Niste prijavljeni pomoću računa koji sadrži zadani direktorij, kao što je contoso.onmicrosoft.com u potpisu, kao što je admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="b416c-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="b416c-106">Prije brisanja uklonite sve aktivne aplikacije u direktoriju.</span><span class="sxs-lookup"><span data-stu-id="b416c-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="b416c-107">Da biste uklonili aktivne aplikacije, dođite do registracija aplikacija i uklonite postojeće aplikacije.</span><span class="sxs-lookup"><span data-stu-id="b416c-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="b416c-108">Ne postoje aktivne pretplate za bilo koji Microsoftov internetski servis, kao što su Microsoft Azure, Office 365 ili Azure AD Premium pridruženi direktoriju.</span><span class="sxs-lookup"><span data-stu-id="b416c-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="b416c-109">Prenesite pretplate ili ubrzajte otkazivanje aktivnih pretplata putem podrške za Azure i naplate.</span><span class="sxs-lookup"><span data-stu-id="b416c-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="b416c-110">Dodatne informacije o otkazu pretplate na Office 365 i Azure.</span><span class="sxs-lookup"><span data-stu-id="b416c-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="b416c-111">Upute za povezivanje ili dodavanje postojeće pretplate na klijenta potražite u članku [pridruživanje ili dodavanje pretplate Azure u klijenta za Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="b416c-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="b416c-112">Nema aktivne licence.</span><span class="sxs-lookup"><span data-stu-id="b416c-112">There are no Active license.</span></span> <span data-ttu-id="b416c-113">Da biste uklonili licence, pročitajte članak [Kako ukloniti pretplatu da biste uklonili licencu](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="b416c-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="b416c-114">Nema drugih aktivnih korisnika u imeniku osim sebe kao globalnog administratora prilikom pokušaja brisanja oglasa Azure.</span><span class="sxs-lookup"><span data-stu-id="b416c-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="b416c-115">Uklonite sve druge aktivne korisnike, a sve ovisnosti o prilagođenom nazivu domene u zakupcu moraju biti uklonjene, kao što su korisnici koji su stvoreni uz admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="b416c-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="b416c-116">Detaljne upute za:</span><span class="sxs-lookup"><span data-stu-id="b416c-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="b416c-117">Brisanje "Azure Active Directory" ili "pretplata" potražite u članku [Brisanje servisa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="b416c-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="b416c-118">Uklanjanje aplikacija u direktoriju potražite u članku [Uklanjanje aplikacija](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="b416c-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
