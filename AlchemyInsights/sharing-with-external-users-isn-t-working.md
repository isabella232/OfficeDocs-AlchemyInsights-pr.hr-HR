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
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582767"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="ed085-102">Rješavanje problema sa zajedničkim korištenjem sadržaja sustava SharePoint s vanjskim korisnicima</span><span class="sxs-lookup"><span data-stu-id="ed085-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="ed085-103">Provjerite je li vanjsko zajedničko korištenje uključeno za vašu tvrtku ili ustanovu:</span><span class="sxs-lookup"><span data-stu-id="ed085-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="ed085-104">Otvorite [stranicu dodaci za &amp; servise u centru za administratore sustava Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), a zatim kliknite **Web- mjesta**.</span><span class="sxs-lookup"><span data-stu-id="ed085-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="ed085-105">Provjerite je li postavka uključena u "Uključeno".</span><span class="sxs-lookup"><span data-stu-id="ed085-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="ed085-106">Ako je odabrana mogućnost "Samo postojeći vanjski korisnici", provjerite je li vanjski korisnik naveden u centru za administratore sustava Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ed085-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="ed085-107">Provjerite je li vanjsko zajedničko korištenje uključeno za web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="ed085-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="ed085-108">Za klasičnu zbirku web-mjesta:</span><span class="sxs-lookup"><span data-stu-id="ed085-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="ed085-109">U novom centru za administratore sustava SharePoint u lijevom oknu kliknite **web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="ed085-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="ed085-110">Odaberite web-mjesto ili web-mjesta, a zatim na vrpci kliknite **Zajedničko korištenje**.</span><span class="sxs-lookup"><span data-stu-id="ed085-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="ed085-111">Za timsko web-mjesto koje pripada grupi Microsoft 365 ili komunikacijskom web-mjestu:</span><span class="sxs-lookup"><span data-stu-id="ed085-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="ed085-112">Te nove vrste web-mjesta imaju istu postavku zajedničkog korištenja kao postavka na razini tvrtke ili ustanove, osim ako postavka na razini tvrtke ili ustanove omogućuje zajedničko korištenje datoteka pomoću veza koje ne zahtijevaju prijavu.</span><span class="sxs-lookup"><span data-stu-id="ed085-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="ed085-113">U tom slučaju web-mjesta dopuštaju zajedničko korištenje s novim i postojećim vanjskim korisnicima koji se prijavljuju.</span><span class="sxs-lookup"><span data-stu-id="ed085-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="ed085-114">Da biste promijenili postavku za određena web-mjesta, koristite novi centar za administratore sustava SharePoint ili PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ed085-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="ed085-115">[Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="ed085-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="ed085-116">Postavka vanjskog zajedničkog korištenja za bilo koje web-mjesto može biti restriktivnija od postavke na razini vaše organizacije, ali ne i popustljivija od postavke na razini tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="ed085-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

