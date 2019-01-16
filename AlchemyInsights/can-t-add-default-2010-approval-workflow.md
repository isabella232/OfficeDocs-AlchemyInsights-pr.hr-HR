---
title: Nije moguće dodati zadani tijek rada za odobrenje 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279578"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="fb108-102">Nije moguće dodati zadani tijek rada za odobrenje 2010</span><span class="sxs-lookup"><span data-stu-id="fb108-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="fb108-103">U zbirke web-mjesta Microsoft SharePoint globalno ponovno iskoristiv tijek rada (na primjer "odobrenje - SharePoint 2010") ne može dodati na popis ili biblioteku.</span><span class="sxs-lookup"><span data-stu-id="fb108-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="fb108-104">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="fb108-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="fb108-105">Otvorite web-mjesto korijena zbirke web-mjesta SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="fb108-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="fb108-106">Pod **Objekti web-mjesta**odaberite **tijekova rada**.</span><span class="sxs-lookup"><span data-stu-id="fb108-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="fb108-107">U sekciji **Novo** vrpce **tijekove rada** , odaberite **Tijek rada za ponovno iskoristiv**.</span><span class="sxs-lookup"><span data-stu-id="fb108-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="fb108-p101">**Stvaranje tijeka rada ponovno iskoristiv** obrascu unesite naziv \* \*\*Repair2010\*\*\*. Za **Vrstu Platform**odaberite **Tijeka rada sustava SharePoint 2010**, a zatim odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="fb108-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="fb108-110">U odjeljak **spremiti** vrpce **tijeka rada** odaberite **Objavi**.</span><span class="sxs-lookup"><span data-stu-id="fb108-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="fb108-p102">U odjeljku **Upravljanje** vrpce **tijeka rada** , odaberite **Objaviti globalno**. U dijaloškom okviru potvrda koja se pojavljuje odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="fb108-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="fb108-p103">U web-pregledniku, pronađite na web-mjestu korijena zbirke web-mjesta i pristup **Postavkama web-mjesta** \> **Značajke zbirke web-mjesta**. Zatim, Preklopi značajka **tijekova rada** :</span><span class="sxs-lookup"><span data-stu-id="fb108-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="fb108-115">· Značajka je *aktivirano* , kliknite **Deaktiviraj,** a zatim kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="fb108-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="fb108-116">· Značajka je *Deactivated* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="fb108-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="fb108-117">Za dodatne informacije pogledajte sljedeći [članak](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="fb108-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

