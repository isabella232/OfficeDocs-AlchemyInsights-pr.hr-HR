---
title: Zajedničko korištenje s vanjskim korisnicima ne funkcionira
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767241"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="24b88-102">Rješavanje problema sa zajedničkim korištenjem sadržaja sustava SharePoint s vanjskim korisnicima</span><span class="sxs-lookup"><span data-stu-id="24b88-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="24b88-103">Provjerite je li vanjsko zajedničko korištenje uključeno za vašu tvrtku ili ustanovu:</span><span class="sxs-lookup"><span data-stu-id="24b88-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="24b88-104">Idite na [ &amp; stranicu Dodaci za usluge u centru za administratore sustava Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), a zatim kliknite **Web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="24b88-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="24b88-105">Provjerite je li postavka uključena u "Uključeno".</span><span class="sxs-lookup"><span data-stu-id="24b88-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="24b88-106">Ako je odabrano "Samo postojeći vanjski korisnici", provjerite je li vanjski korisnik naveden u centru za administratore sustava Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="24b88-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="24b88-107">Provjerite je li vanjsko zajedničko korištenje uključeno za web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="24b88-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="24b88-108">Za klasičnu zbirku web-mjesta:</span><span class="sxs-lookup"><span data-stu-id="24b88-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="24b88-109">U novom centru za administratore sustava SharePoint u lijevom oknu kliknite **web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="24b88-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="24b88-110">Odaberite web-mjesto ili web-mjesto, a zatim na vrpci kliknite **Zajedničko korištenje**.</span><span class="sxs-lookup"><span data-stu-id="24b88-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="24b88-111">Za timsko web-mjesto koje pripada grupi sustava Office 365 ili komunikacijskom web-mjestu:</span><span class="sxs-lookup"><span data-stu-id="24b88-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="24b88-112">Te nove vrste web-mjesta imaju istu postavku zajedničkog korištenja kao i postavka na razini tvrtke ili ustanove, osim ako postavka na razini tvrtke ili ustanove dopušta zajedničko korištenje datoteka pomoću veza koje ne zahtijevaju prijavu.</span><span class="sxs-lookup"><span data-stu-id="24b88-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="24b88-113">U tom slučaju web-mjesta omogućuju zajedničko korištenje s novim i postojećim vanjskim korisnicima koji se prijavljuju.</span><span class="sxs-lookup"><span data-stu-id="24b88-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="24b88-114">Da biste promijenili postavku za određena web-mjesta, koristite novi centar za administratore sustava SharePoint ili PowerShell.</span><span class="sxs-lookup"><span data-stu-id="24b88-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="24b88-115">[Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="24b88-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="24b88-116">Postavka vanjskog zajedničkog korištenja za bilo koje web-mjesto može biti restriktivnija od postavke na razini tvrtke ili ustanove, ali ne i popustljivija od postavke na razini organizacije.</span><span class="sxs-lookup"><span data-stu-id="24b88-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

