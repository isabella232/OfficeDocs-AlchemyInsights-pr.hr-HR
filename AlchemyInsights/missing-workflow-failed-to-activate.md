---
title: Nedostaje tijek rada nije uspio aktivirati
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29461305"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="c6dba-102">Nedostaje tijek rada nije uspio aktivirati</span><span class="sxs-lookup"><span data-stu-id="c6dba-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="c6dba-103">U zbirke web-mjesta Microsoft SharePoint globalno ponovno iskoristiv tijek rada (na primjer "odobrenje - SharePoint 2010") ne može dodati na popis ili biblioteku.</span><span class="sxs-lookup"><span data-stu-id="c6dba-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="c6dba-104">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="c6dba-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="c6dba-105">Otvorite web-mjesto korijena zbirke web-mjesta SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="c6dba-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="c6dba-106">Pod **Objekti web-mjesta**odaberite **tijekova rada**.</span><span class="sxs-lookup"><span data-stu-id="c6dba-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="c6dba-107">U sekciji **Novo** vrpce **tijekove rada** , odaberite **Tijek rada za ponovno iskoristiv**.</span><span class="sxs-lookup"><span data-stu-id="c6dba-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="c6dba-p101">**Stvaranje tijeka rada ponovno iskoristiv** obrascu unesite naziv \*\* *Repair2010* \*\*. Za **Vrstu Platform**kliknite **Tijeka rada sustava SharePoint 2010**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="c6dba-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="c6dba-110">U odjeljak **spremiti** vrpce **tijeka rada** odaberite **Objavi**.</span><span class="sxs-lookup"><span data-stu-id="c6dba-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="c6dba-p102">U odjeljku **Upravljanje** vrpce **tijeka rada** , odaberite **Objaviti globalno**. U dijaloškom okviru potvrda koja se pojavljuje odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="c6dba-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="c6dba-p103">U web-pregledniku, pronađite na web-mjestu korijena zbirke web-mjesta i pristup **Postavkama web-mjesta** \> **Značajke zbirke web-mjesta**. Zatim, Preklopi značajka **tijekova rada** :</span><span class="sxs-lookup"><span data-stu-id="c6dba-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="c6dba-115">· Značajka je *aktivirano* , kliknite **Deaktiviraj,** a zatim kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="c6dba-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="c6dba-116">· Značajka je *Deactivated* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="c6dba-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="c6dba-117">Za dodatne informacije pogledajte sljedeći [članak](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c6dba-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

