---
title: Nestanak tijeka rada nije uspio aktivirati
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36753788"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="89f79-102">Nestanak tijeka rada nije uspio aktivirati</span><span class="sxs-lookup"><span data-stu-id="89f79-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="89f79-103">U zbirci web-mjesta programa Microsoft SharePoint ne možete dodati globalni tijek rada koji se može ponovno koristiti (kao što je "odobrenje-SharePoint 2010") na popis ili biblioteku.</span><span class="sxs-lookup"><span data-stu-id="89f79-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="89f79-104">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="89f79-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="89f79-105">Otvorite korijensku web-lokaciju zbirke web-mjesta u programu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="89f79-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="89f79-106">U odjeljku **objekti web-mjesta**odaberite **tijekove rada**.</span><span class="sxs-lookup"><span data-stu-id="89f79-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="89f79-107">U **novom** odjeljku vrpce **Tijekovi rada** odaberite **Ponovno iskoristiv tijek rada**.</span><span class="sxs-lookup"><span data-stu-id="89f79-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="89f79-108">**Da biste** unijeli naziv \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="89f79-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="89f79-109">Za **vrstu platforme**kliknite **SharePoint 2010 Workflow**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="89f79-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="89f79-110">U odjeljku **Spremi** na vrpci **tijeka rada** odaberite **Objavi**.</span><span class="sxs-lookup"><span data-stu-id="89f79-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="89f79-111">U odjeljku **Upravljanje** vrpcom **tijeka rada** odaberite **Objavi globalno**.</span><span class="sxs-lookup"><span data-stu-id="89f79-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="89f79-112">U potvrdnom dijaloškom okviru koji se pojavi odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="89f79-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="89f79-113">U web-pregledniku Pronađite korijensku web-lokaciju zbirke web-mjesta, a zatim pristupite **značajkama zbirke web**-mjesta za **postavku** \> web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="89f79-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="89f79-114">Zatim uključite značajku **tijekova rada** :</span><span class="sxs-lookup"><span data-stu-id="89f79-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="89f79-115">· Ako je značajka *aktivirana* , kliknite " **Deaktiviraj",** a zatim kliknite " **Aktiviraj**".</span><span class="sxs-lookup"><span data-stu-id="89f79-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="89f79-116">· Ako je značajka *deaktivirana* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="89f79-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="89f79-117">Dodatne informacije potražite u sljedećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="89f79-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

