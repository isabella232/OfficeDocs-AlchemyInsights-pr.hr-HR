---
title: Dijeljenje s vanjskim korisnicima ne radi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502223"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="eece3-102">Rješavanje problema s dijeljenjem SharePointovog sadržaja s vanjskim korisnicima</span><span class="sxs-lookup"><span data-stu-id="eece3-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="eece3-103">Provjerite je li vanjsko zajedničko korištenje uključeno za vašu organizaciju:</span><span class="sxs-lookup"><span data-stu-id="eece3-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="eece3-104">Idite na [stranicu dodataka &amp; za usluge u centru za administraciju Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i kliknite **web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="eece3-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="eece3-105">Provjerite je li postavka uključena u "uključeno".</span><span class="sxs-lookup"><span data-stu-id="eece3-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="eece3-106">Ako je odabran "samo postojeći vanjski korisnici", provjerite je li vanjski korisnik naveden u centru za administraciju Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="eece3-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="eece3-107">Provjerite je li vanjsko dijeljenje uključeno za web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="eece3-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="eece3-108">Za klasičnu zbirku web-mjesta:</span><span class="sxs-lookup"><span data-stu-id="eece3-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="eece3-109">U novom centru za administraciju sustava SharePoint u lijevom oknu kliknite **web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="eece3-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="eece3-110">Odaberite web-mjesto ili web-mjesta, a zatim na vrpci kliknite **dijeljenje**.</span><span class="sxs-lookup"><span data-stu-id="eece3-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="eece3-111">Za timsko web-mjesto koje pripada grupi sustava Office 365 ili web-mjestu za komunikaciju:</span><span class="sxs-lookup"><span data-stu-id="eece3-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="eece3-112">Te nove vrste web-mjesta imaju jednaku postavku dijeljenja kao i postavku za vašu organizaciju, osim ako postavka na razini organizacije omogućuje dijeljenje datoteka pomoću veza koje ne zahtijevaju prijavu.</span><span class="sxs-lookup"><span data-stu-id="eece3-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="eece3-113">U tom slučaju web-mjesta dopuštaju dijeljenje s novim i postojećim vanjskim korisnicima koji se prijave.</span><span class="sxs-lookup"><span data-stu-id="eece3-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="eece3-114">Da biste promijenili postavku za određena web-mjesta, upotrijebite novi centar za administraciju sustava SharePoint ili PowerShell.</span><span class="sxs-lookup"><span data-stu-id="eece3-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="eece3-115">[Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="eece3-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="eece3-116">Postavka vanjskog dijeljenja za bilo koje web-mjesto može biti restriktivnija od postavke u cijeloj organizaciji, ali ne više popustljiva od postavke u cijeloj organizaciji.</span><span class="sxs-lookup"><span data-stu-id="eece3-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

