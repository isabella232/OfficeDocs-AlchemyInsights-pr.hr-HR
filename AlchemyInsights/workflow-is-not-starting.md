---
title: Tijek rada se ne započinje
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403735"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="2d24f-102">Tijek rada se ne započinje</span><span class="sxs-lookup"><span data-stu-id="2d24f-102">Workflow is not starting</span></span>

- <span data-ttu-id="2d24f-103">Tijekovi rada sustava SharePoint 2010 i SharePoint 2013 ne počinju.</span><span class="sxs-lookup"><span data-stu-id="2d24f-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="2d24f-104">Ako se tijek rada ne započinje, možda postoji privremeni problem sa servisom u kojem korisnici mogu naiči na povremene kašnjenje tijeka rada.</span><span class="sxs-lookup"><span data-stu-id="2d24f-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="2d24f-105">Provjerite [nadzornu ploču stanja servisa](https://admin.microsoft.com/AdminPortal/Home/servicehealth) da biste vidjeli utječe li vaša tvrtka ili ustanova na to.</span><span class="sxs-lookup"><span data-stu-id="2d24f-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="2d24f-106">Ako je prošlo više od 24 sata od kada ste prvi put vidjeli taj problem, prijavite kartu za podršku.</span><span class="sxs-lookup"><span data-stu-id="2d24f-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="2d24f-107">U mnogim slučajevima već radimo na rješenju.</span><span class="sxs-lookup"><span data-stu-id="2d24f-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2d24f-108">Dajte nam najmanje 24 sata da dovršimo rješenje.</span><span class="sxs-lookup"><span data-stu-id="2d24f-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="2d24f-109">Tijekovi rada sustava SharePoint 2010 odgođeni su pri pokretanju.</span><span class="sxs-lookup"><span data-stu-id="2d24f-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="2d24f-110">To se događa ako se tijek rada pokreće u velikim grupama.</span><span class="sxs-lookup"><span data-stu-id="2d24f-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="2d24f-111">(na primjer, kada se doda nekoliko stavki odjednom).</span><span class="sxs-lookup"><span data-stu-id="2d24f-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="2d24f-112">Tijekovi rada nisu dizajnirani za pokretanje u stvarnom vremenu, pa je kašnjenje ponašanje po dizajnu.</span><span class="sxs-lookup"><span data-stu-id="2d24f-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="2d24f-113">Ako je tijek rada složen jezik oznake extensible Object Markup Language (XMOL), sastavljanje može biti sporo.</span><span class="sxs-lookup"><span data-stu-id="2d24f-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="2d24f-114">Pogledajte [ovaj](https://support.microsoft.com//kb/3043697) članak.</span><span class="sxs-lookup"><span data-stu-id="2d24f-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="2d24f-115">Trebali biste pojednostavniti tijek rada ili ga redizajnirati pomoću vrste platforme Tijek rada sustava Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="2d24f-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="2d24f-116">Ako je povijest tijeka rada narasla, možda želite očistiti stavke ili stvoriti novi popis povijesti.</span><span class="sxs-lookup"><span data-stu-id="2d24f-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="2d24f-117">Dodatne informacije : [Čišćenje povijesti tijeka rada](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="2d24f-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="2d24f-118">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="2d24f-118">Related topics</span></span>
<span data-ttu-id="2d24f-119">Želite li isprobati Microsoft Flow u sustavu SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="2d24f-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="2d24f-120">Stvaranje tijeka</span><span class="sxs-lookup"><span data-stu-id="2d24f-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="2d24f-121">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="2d24f-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
