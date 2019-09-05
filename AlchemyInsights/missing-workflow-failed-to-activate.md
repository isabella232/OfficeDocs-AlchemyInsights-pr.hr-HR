---
title: Nedostaje tijek rada nije uspio aktivirati
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753788"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="ca1bd-102">Nedostaje tijek rada nije uspio aktivirati</span><span class="sxs-lookup"><span data-stu-id="ca1bd-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="ca1bd-103">U zbirke web-mjesta Microsoft SharePoint globalno ponovno iskoristiv tijek rada (na primjer "odobrenje - SharePoint 2010") ne može dodati na popis ili biblioteku.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="ca1bd-104">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="ca1bd-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="ca1bd-105">Otvorite web-mjesto korijena zbirke web-mjesta SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="ca1bd-106">Pod **Objekti web-mjesta**odaberite **tijekova rada**.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="ca1bd-107">U sekciji **Novo** vrpce **tijekove rada** , odaberite **Tijek rada za ponovno iskoristiv**.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="ca1bd-108">**Stvaranje tijeka rada ponovno iskoristiv** obrascu unesite naziv \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="ca1bd-109">Za **Vrstu Platform**kliknite **Tijeka rada sustava SharePoint 2010**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="ca1bd-110">U odjeljak **spremiti** vrpce **tijeka rada** odaberite **Objavi**.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="ca1bd-111">U odjeljku **Upravljanje** vrpce **tijeka rada** , odaberite **Objaviti globalno**.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="ca1bd-112">U dijaloškom okviru potvrda koja se pojavljuje odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="ca1bd-113">U web-pregledniku, pronađite na web-mjestu korijena zbirke web-mjesta i pristup **Postavkama web-mjesta** \> **Značajke zbirke web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="ca1bd-114">Zatim, Preklopi značajka **tijekova rada** :</span><span class="sxs-lookup"><span data-stu-id="ca1bd-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="ca1bd-115">· Značajka je *aktivirano* , kliknite **Deaktiviraj,** a zatim kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="ca1bd-116">· Značajka je *Deactivated* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="ca1bd-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="ca1bd-117">Za dodatne informacije pogledajte sljedeći [članak](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="ca1bd-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

