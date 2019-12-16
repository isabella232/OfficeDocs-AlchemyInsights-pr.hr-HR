---
title: Nije moguće dodati 2010 tijek rada za odobrenje
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049545"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="55e21-102">Nije moguće dodati 2010 tijek rada za odobrenje</span><span class="sxs-lookup"><span data-stu-id="55e21-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="55e21-103">U zbirci web-mjesta programa Microsoft SharePoint ne možete dodati globalni tijek rada koji se može ponovno koristiti (kao što je "odobrenje-SharePoint 2010") na popis ili biblioteku.</span><span class="sxs-lookup"><span data-stu-id="55e21-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="55e21-104">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="55e21-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="55e21-105">Otvorite korijensku web-lokaciju zbirke web-mjesta u programu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="55e21-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="55e21-106">U odjeljku **objekti web-mjesta**odaberite **tijekove rada**.</span><span class="sxs-lookup"><span data-stu-id="55e21-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="55e21-107">U **novom** odjeljku vrpce **Tijekovi rada** odaberite **Ponovno iskoristiv tijek rada**.</span><span class="sxs-lookup"><span data-stu-id="55e21-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="55e21-108">**Da biste** unijeli naziv \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="55e21-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="55e21-109">Za **vrstu platforme**kliknite **SharePoint 2010 Workflow**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="55e21-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="55e21-110">U odjeljku **Spremi** na vrpci **tijeka rada** odaberite **Objavi**.</span><span class="sxs-lookup"><span data-stu-id="55e21-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="55e21-111">U odjeljku **Upravljanje** vrpcom **tijeka rada** odaberite **Objavi globalno**.</span><span class="sxs-lookup"><span data-stu-id="55e21-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="55e21-112">U potvrdnom dijaloškom okviru koji se pojavi odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="55e21-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="55e21-113">U web-pregledniku Pronađite korijensku web-lokaciju zbirke web-mjesta, a zatim pristupite **značajkama zbirke web**-mjesta za **postavku** \> web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="55e21-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="55e21-114">Uključivanje/isključivanje značajke **tijekova rada** :</span><span class="sxs-lookup"><span data-stu-id="55e21-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="55e21-115">· Ako je značajka *aktivirana* , kliknite " **Deaktiviraj",** a zatim kliknite " **Aktiviraj**".</span><span class="sxs-lookup"><span data-stu-id="55e21-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="55e21-116">· Ako je značajka *deaktivirana* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="55e21-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="55e21-117">Dodatne informacije potražite u sljedećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="55e21-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

