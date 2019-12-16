---
title: Nestanak tijeka rada nije uspio aktivirati
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052605"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="66abe-102">Nestanak tijeka rada nije uspio aktivirati</span><span class="sxs-lookup"><span data-stu-id="66abe-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="66abe-103">U zbirci web-mjesta programa Microsoft SharePoint ne možete dodati globalni tijek rada koji se može ponovno koristiti (kao što je "odobrenje-SharePoint 2010") na popis ili biblioteku.</span><span class="sxs-lookup"><span data-stu-id="66abe-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="66abe-104">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="66abe-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="66abe-105">Otvorite korijensku web-lokaciju zbirke web-mjesta u programu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="66abe-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="66abe-106">U odjeljku **objekti web-mjesta**odaberite **tijekove rada**.</span><span class="sxs-lookup"><span data-stu-id="66abe-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="66abe-107">U **novom** odjeljku vrpce **Tijekovi rada** odaberite **Ponovno iskoristiv tijek rada**.</span><span class="sxs-lookup"><span data-stu-id="66abe-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="66abe-108">**Da biste** unijeli naziv \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="66abe-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="66abe-109">Za **vrstu platforme**kliknite **SharePoint 2010 Workflow**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="66abe-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="66abe-110">U odjeljku **Spremi** na vrpci **tijeka rada** odaberite **Objavi**.</span><span class="sxs-lookup"><span data-stu-id="66abe-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="66abe-111">U odjeljku **Upravljanje** vrpcom **tijeka rada** odaberite **Objavi globalno**.</span><span class="sxs-lookup"><span data-stu-id="66abe-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="66abe-112">U potvrdnom dijaloškom okviru koji se pojavi odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="66abe-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="66abe-113">U web-pregledniku Pronađite korijensku web-lokaciju zbirke web-mjesta, a zatim pristupite **značajkama zbirke web**-mjesta za **postavku** \> web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="66abe-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="66abe-114">Zatim uključite značajku **tijekova rada** :</span><span class="sxs-lookup"><span data-stu-id="66abe-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="66abe-115">· Ako je značajka *aktivirana* , kliknite " **Deaktiviraj",** a zatim kliknite " **Aktiviraj**".</span><span class="sxs-lookup"><span data-stu-id="66abe-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="66abe-116">· Ako je značajka *deaktivirana* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="66abe-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="66abe-117">Dodatne informacije potražite u sljedećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="66abe-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

