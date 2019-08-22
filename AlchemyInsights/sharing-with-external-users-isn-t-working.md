---
title: Zajedničko korištenje s vanjskim korisnicima ne radi
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502223"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="6ed31-102">Riješite probleme s vanjskim korisnicima dijeljenje SharePoint sadržaja</span><span class="sxs-lookup"><span data-stu-id="6ed31-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="6ed31-103">Provjerite je li vanjski je uključeno zajedničko korištenje vaše organizacije:</span><span class="sxs-lookup"><span data-stu-id="6ed31-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="6ed31-104">Idite na [Services &amp; stranici dodaci u centru za administraciju Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), i kliknite **mjesta**.</span><span class="sxs-lookup"><span data-stu-id="6ed31-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="6ed31-105">Provjerite je li postavka uključena za "Na."</span><span class="sxs-lookup"><span data-stu-id="6ed31-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="6ed31-106">Ako odabrano je "Samo postojeće vanjski korisnici", provjerite vanjskog korisnika navedene u centru za administraciju Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6ed31-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="6ed31-107">Provjerite vanjske dijeljenja uključen za web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="6ed31-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="6ed31-108">Klasični zbirke stranica:</span><span class="sxs-lookup"><span data-stu-id="6ed31-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="6ed31-109">Novi centar admin SharePoint, u lijevom oknu kliknite **mjesta**.</span><span class="sxs-lookup"><span data-stu-id="6ed31-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="6ed31-110">Odaberite web-mjesta ili web-mjesta i na vrpci kliknite **zajedničko korištenje**.</span><span class="sxs-lookup"><span data-stu-id="6ed31-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="6ed31-111">Za web-mjesto tima koji pripada grupi Office 365 ili komunikacije web-mjesta:</span><span class="sxs-lookup"><span data-stu-id="6ed31-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="6ed31-112">Ove nove vrste web-mjesta imaju na isti zajedničko korištenje postavljanje kao postavku nivou organizacije, osim ako postavka nivou organizacije omogućuje zajedničko korištenje datoteka pomoću veze koje ne zahtijevaju prijavu.</span><span class="sxs-lookup"><span data-stu-id="6ed31-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="6ed31-113">U tom slučaju web-mjesta Dopusti zajedničko korištenje nove i postojeće vanjski korisnici koji se prijaviti.</span><span class="sxs-lookup"><span data-stu-id="6ed31-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="6ed31-114">Da biste promijenili postavke za određena web-mjesta, koristite novi SharePoint administraciju centar ili PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6ed31-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="6ed31-115">[Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="6ed31-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="6ed31-116">Vanjski zajedničko korištenje postavka za bilo koje web-mjesto može biti šira od postavku nivou organizacije, ali ne više čemu od postavke nivou organizacije.</span><span class="sxs-lookup"><span data-stu-id="6ed31-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

