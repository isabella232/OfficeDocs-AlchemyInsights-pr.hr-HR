---
title: Zajedničko korištenje s vanjskim korisnicima ne funkcionira
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691567"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="7bd9f-102">Rješavanje problema s zajedničkim korištenjem sadržaja sustava SharePoint s vanjskim korisnicima</span><span class="sxs-lookup"><span data-stu-id="7bd9f-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="7bd9f-103">Provjerite je li za vašu tvrtku ili ustanovu uključena vanjsko zajedničko korištenje:</span><span class="sxs-lookup"><span data-stu-id="7bd9f-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="7bd9f-104">Idite na [ &amp; stranicu Dodaci servisa u centru za administratore sustava Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), a zatim kliknite **web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="7bd9f-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="7bd9f-105">Provjerite je li postavka pretvorena u "uključeno".</span><span class="sxs-lookup"><span data-stu-id="7bd9f-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="7bd9f-106">Ako je odabrana mogućnost "samo postojeći vanjski korisnici", provjerite je li vanjski korisnik naveden u centru za administratore sustava Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7bd9f-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="7bd9f-107">Provjerite je li vanjsko zajedničko korištenje uključeno za web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="7bd9f-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="7bd9f-108">Za klasičnu zbirku web-mjesta:</span><span class="sxs-lookup"><span data-stu-id="7bd9f-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="7bd9f-109">U novom centru za administratore sustava SharePoint u desnom oknu kliknite **web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="7bd9f-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="7bd9f-110">Odaberite web-mjesto ili web-mjesta, a zatim na vrpci kliknite **zajedničko korištenje**.</span><span class="sxs-lookup"><span data-stu-id="7bd9f-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="7bd9f-111">Za timsko web-mjesto koje pripada grupi Microsoft 365 ili komunikacijskom web-mjestu:</span><span class="sxs-lookup"><span data-stu-id="7bd9f-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="7bd9f-112">Te nove vrste web-mjesta imaju istu postavku zajedničkog korištenja kao postavke za cijelu tvrtku ili ustanovu, osim ako postavka u sklopu tvrtke ili ustanove ne dopušta zajedničko korištenje datoteka pomoću veza koje ne zahtijevaju prijavu.</span><span class="sxs-lookup"><span data-stu-id="7bd9f-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="7bd9f-113">U ovom slučaju web-mjesta omogućuju zajedničko korištenje s novim i postojećim vanjskim korisnicima koji se prijavljuju.</span><span class="sxs-lookup"><span data-stu-id="7bd9f-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="7bd9f-114">Da biste promijenili postavku za određena web-mjesta, koristite novi centar za administratore sustava SharePoint ili PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7bd9f-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="7bd9f-115">[Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="7bd9f-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="7bd9f-116">Postavka vanjskog zajedničkog korištenja za bilo koje web-mjesto može biti restriktivniji od postavke za cijelu tvrtku ili ustanovu, ali ne i više nego što je postavka u cijelom tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="7bd9f-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

