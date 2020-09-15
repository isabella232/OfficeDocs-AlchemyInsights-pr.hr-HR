---
title: Nije uspjelo Aktiviranje tijeka rada koji nema
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667078"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="bb33a-102">Nije uspjelo Aktiviranje tijeka rada koji nema</span><span class="sxs-lookup"><span data-stu-id="bb33a-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="bb33a-103">U zbirci web-mjesta sustava Microsoft SharePoint ne možete dodati globalni tijek rada za ponovno korištenje (kao što je "odobrenje-SharePoint 2010") na popis ili u biblioteku.</span><span class="sxs-lookup"><span data-stu-id="bb33a-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="bb33a-104">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="bb33a-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="bb33a-105">Otvorite korijensko web-mjesto zbirke web-mjesta u sustavu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="bb33a-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="bb33a-106">U odjeljku **objekti web-mjesta**odaberite **Tijekovi rada**.</span><span class="sxs-lookup"><span data-stu-id="bb33a-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="bb33a-107">U **novom** odjeljku vrpce **tijekova rada** odaberite **Ponovno iskoristiv tijek rada**.</span><span class="sxs-lookup"><span data-stu-id="bb33a-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="bb33a-108">Na obrascu **Stvaranje ponovno iskoristivog tijeka rada** unesite naziv \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="bb33a-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="bb33a-109">Za **vrstu platforme**kliknite **tijek rada sustava SharePoint 2010**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="bb33a-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="bb33a-110">U odjeljku **Spremanje** na vrpci **tijeka rada** odaberite **Objavi**.</span><span class="sxs-lookup"><span data-stu-id="bb33a-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="bb33a-111">U odjeljku **Upravljanje** na vrpci **tijeka rada** odaberite **Objavi globalno**.</span><span class="sxs-lookup"><span data-stu-id="bb33a-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="bb33a-112">U dijaloškom okviru za potvrdu koji će se prikazati odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="bb33a-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="bb33a-113">U web-pregledniku Pronađite korijensko web-mjesto zbirke web-mjesta, a zatim **Site Settings** \> **značajke zbirke web-mjesta**za postavljanje web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="bb33a-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="bb33a-114">Zatim preklopni značajku **tijekova rada** :</span><span class="sxs-lookup"><span data-stu-id="bb33a-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="bb33a-115">· Ako je značajka  *aktivirana*  , kliknite **Deaktiviraj,** a zatim **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="bb33a-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="bb33a-116">· Ako je značajka  *deaktivirana*  , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="bb33a-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="bb33a-117">Dodatne informacije potražite u sljedećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="bb33a-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

