---
title: Nije moguće dodati tijek rada za odobrenje 2010.
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582839"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="38edd-102">Nije moguće dodati tijek rada za odobrenje 2010.</span><span class="sxs-lookup"><span data-stu-id="38edd-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="38edd-103">U zbirci web-mjesta sustava Microsoft SharePoint ne možete dodati globalno ponovno upotrebljiv tijek rada (kao što je "Odobrenje - SharePoint 2010") na popis ili u biblioteci.</span><span class="sxs-lookup"><span data-stu-id="38edd-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="38edd-104">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="38edd-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="38edd-105">Otvorite korijensko web-mjesto zbirke web-mjesta u programu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="38edd-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="38edd-106">U **odjeljku Objekti web-mjesta**odaberite **Tijekovi rada**.</span><span class="sxs-lookup"><span data-stu-id="38edd-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="38edd-107">U odjeljku **Novo** na **vrpci Tijekovi rada** odaberite **Ponovno upotrebljiva tijek rada**.</span><span class="sxs-lookup"><span data-stu-id="38edd-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="38edd-108">Na obrascu **Stvaranje tijeka rada za višekratnu upotrebu** unesite naziv \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="38edd-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="38edd-109">Za **vrstu platforme**kliknite Tijek rada sustava **SharePoint 2010**, a zatim **U redu**.</span><span class="sxs-lookup"><span data-stu-id="38edd-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="38edd-110">U odjeljku **Spremanje** na vrpci **Tijek rada** odaberite **Objavi**.</span><span class="sxs-lookup"><span data-stu-id="38edd-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="38edd-111">U odjeljku **Upravljanje** na vrpci **Tijek rada** odaberite **Objavi globalno**.</span><span class="sxs-lookup"><span data-stu-id="38edd-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="38edd-112">U dijaloškom okviru za potvrdu koji će se pojaviti odaberite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="38edd-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="38edd-113">U web-pregledniku pronađite korijensko web-mjesto zbirke web-mjesta, a zatim **pristupite značajkama zbirke web-mjesta postavki** \> **web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="38edd-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="38edd-114">Uključivanje/isključivanje značajke **Tijekovi rada:**</span><span class="sxs-lookup"><span data-stu-id="38edd-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="38edd-115">· Ako je značajka *aktivirana* , kliknite **Deaktiviraj,** a zatim **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="38edd-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="38edd-116">· Ako je značajka *deaktivirana* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="38edd-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="38edd-117">Za više informacija pogledajte sljedeći [članak](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="38edd-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

