---
title: Nije moguće dodati tijek rada za odobrenje 2010
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748676"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="aa5b6-102">Nije moguće dodati tijek rada za odobrenje 2010</span><span class="sxs-lookup"><span data-stu-id="aa5b6-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="aa5b6-103">U zbirke web-mjesta Microsoft SharePoint globalno ponovno iskoristiv tijek rada (na primjer "odobrenje - SharePoint 2010") ne može dodati na popis ili biblioteku.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="aa5b6-104">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="aa5b6-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="aa5b6-105">Otvorite web-mjesto korijena zbirke web-mjesta SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="aa5b6-106">Pod **Objekti web-mjesta**odaberite **tijekova rada**.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="aa5b6-107">U sekciji **Novo** vrpce **tijekove rada** , odaberite **Tijek rada za ponovno iskoristiv**.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="aa5b6-108">**Stvaranje tijeka rada ponovno iskoristiv** obrascu unesite naziv \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="aa5b6-109">Za **Vrstu Platform**kliknite **Tijeka rada sustava SharePoint 2010**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="aa5b6-110">U odjeljak **spremiti** vrpce **tijeka rada** odaberite **Objavi**.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="aa5b6-111">U odjeljku **Upravljanje** vrpce **tijeka rada** , odaberite **Objaviti globalno**.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="aa5b6-112">U dijaloškom okviru potvrda koja se pojavljuje odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="aa5b6-113">U web-pregledniku, pronađite na web-mjestu korijena zbirke web-mjesta i pristup **Postavkama web-mjesta** \> **Značajke zbirke web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="aa5b6-114">Preklopi značajka **tijekova rada** :</span><span class="sxs-lookup"><span data-stu-id="aa5b6-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="aa5b6-115">· Značajka je *aktivirano* , kliknite **Deaktiviraj,** a zatim kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="aa5b6-116">· Značajka je *Deactivated* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="aa5b6-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="aa5b6-117">Za dodatne informacije pogledajte sljedeći [članak](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="aa5b6-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

