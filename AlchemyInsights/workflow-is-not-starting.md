---
title: Tijek rada se ne pokreće
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794759"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="b50dc-102">Tijek rada se ne pokreće</span><span class="sxs-lookup"><span data-stu-id="b50dc-102">Workflow is not starting</span></span>

- <span data-ttu-id="b50dc-103">Tijekovi rada sustava SharePoint 2010 i SharePoint 2013 ne počinju.</span><span class="sxs-lookup"><span data-stu-id="b50dc-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="b50dc-104">Ako se tijek rada ne pokreće, možda postoji privremeni problem s servisom u kojem korisnici mogu iskusiti povremeni kašnjenje s napretkom tijeka rada.</span><span class="sxs-lookup"><span data-stu-id="b50dc-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="b50dc-105">Provjerite je li vaša tvrtka ili ustanova utjecala na [nadzornu ploču zdravstvenog stanja servisa](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) .</span><span class="sxs-lookup"><span data-stu-id="b50dc-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="b50dc-106">Ako je prošlo više od 24 sata otkad ste prvi put vidjeli taj problem, prijavite karticu za podršku.</span><span class="sxs-lookup"><span data-stu-id="b50dc-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b50dc-107">U mnogim slučajevima već radimo na rješenju.</span><span class="sxs-lookup"><span data-stu-id="b50dc-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b50dc-108">Dodajte nam najmanje 24 sata da biste dovršili rješenje.</span><span class="sxs-lookup"><span data-stu-id="b50dc-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="b50dc-109">Tijekovi rada sustava SharePoint 2010 odgođeni su pri pokretanju.</span><span class="sxs-lookup"><span data-stu-id="b50dc-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="b50dc-110">To se događa ako se tijek rada aktivira u velikim grupama.</span><span class="sxs-lookup"><span data-stu-id="b50dc-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="b50dc-111">(na primjer, kada se nekoliko stavki odmah doda).</span><span class="sxs-lookup"><span data-stu-id="b50dc-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="b50dc-112">Tijekovi rada nisu dizajnirani za izvođenje u stvarnom vremenu, pa je kašnjenje prema dizajnu.</span><span class="sxs-lookup"><span data-stu-id="b50dc-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="b50dc-113">Ako je tijek rada kompleksan Extensible Object Markup Language (XMOL), kompilacija može biti spora.</span><span class="sxs-lookup"><span data-stu-id="b50dc-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="b50dc-114">Provjerite [ovaj](https://support.microsoft.com//kb/3043697) članak.</span><span class="sxs-lookup"><span data-stu-id="b50dc-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="b50dc-115">Trebali biste pojednostavniti tijek rada ili ga ponovno dizajnirati pomoću vrste platforme tijeka rada sustava Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="b50dc-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="b50dc-116">Ako je povijest tijeka rada porasla, možda želite očistiti stavke ili stvoriti novi popis povijesti.</span><span class="sxs-lookup"><span data-stu-id="b50dc-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="b50dc-117">Dodatne informacije: [čišćenje povijesti tijeka rada](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="b50dc-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="b50dc-118">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="b50dc-118">Related topics</span></span>
<span data-ttu-id="b50dc-119">Želite li isprobati Microsoft Flow u sustavu SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="b50dc-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="b50dc-120">Stvaranje toka</span><span class="sxs-lookup"><span data-stu-id="b50dc-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="b50dc-121">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="b50dc-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


