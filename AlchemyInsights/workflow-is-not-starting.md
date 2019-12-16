---
title: Tijek rada se ne započinje
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049329"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="51ff4-102">Tijek rada se ne započinje</span><span class="sxs-lookup"><span data-stu-id="51ff4-102">Workflow is not starting</span></span>

- <span data-ttu-id="51ff4-103">Tijekovi rada sustava SharePoint 2010 i SharePoint 2013 se ne počinju.</span><span class="sxs-lookup"><span data-stu-id="51ff4-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="51ff4-104">Ako se tijek rada ne započinje, možda postoji problem s privremenim servisima u kojem korisnici mogu doživjeti povremene odgode s napretkom tijeka rada.</span><span class="sxs-lookup"><span data-stu-id="51ff4-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="51ff4-105">Provjerite je li vaša tvrtka ili ustanova utjecala na [nadzornu ploču za zdravstvenu službu](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) .</span><span class="sxs-lookup"><span data-stu-id="51ff4-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="51ff4-106">Ako je prošlo više od 24 sata od kada ste prvi put vidjeli ovaj problem, molimo prijavite ulaznicu za podršku.</span><span class="sxs-lookup"><span data-stu-id="51ff4-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="51ff4-107">U mnogim slučajevima već radimo na rješenju.</span><span class="sxs-lookup"><span data-stu-id="51ff4-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="51ff4-108">Molim vas, dajte nam najmanje 24 sata da dovršimo rješenje.</span><span class="sxs-lookup"><span data-stu-id="51ff4-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="51ff4-109">Tijekovi rada sustava SharePoint 2010 odgođeni na početku.</span><span class="sxs-lookup"><span data-stu-id="51ff4-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="51ff4-110">To se događa ako se tijek rada aktivira u velikim serijama.</span><span class="sxs-lookup"><span data-stu-id="51ff4-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="51ff4-111">(na primjer, kada se nekoliko stavki doda odjednom).</span><span class="sxs-lookup"><span data-stu-id="51ff4-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="51ff4-112">Tijekovi rada nisu dizajnirani za izvođenje u realnom vremenu, tako da je odgoda po dizajnu ponašanje.</span><span class="sxs-lookup"><span data-stu-id="51ff4-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="51ff4-113">Ako je tijek rada složen Extensible Object Markup Language (XMOL), kompilacija može biti spora.</span><span class="sxs-lookup"><span data-stu-id="51ff4-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="51ff4-114">Provjerite [ovaj](https://support.microsoft.com//kb/3043697) članak.</span><span class="sxs-lookup"><span data-stu-id="51ff4-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="51ff4-115">Trebali biste pojednostavniti tijek rada ili ga redizajnirati pomoću vrste platforme Microsoft SharePoint 2013 workflow.</span><span class="sxs-lookup"><span data-stu-id="51ff4-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="51ff4-116">Ako je vaša povijest tijeka rada narasla, možda želite očistiti stavke ili stvoriti novi popis povijesti.</span><span class="sxs-lookup"><span data-stu-id="51ff4-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="51ff4-117">Dodatne informacije: [čišćenje povijesti tijeka rada](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="51ff4-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="51ff4-118">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="51ff4-118">Related topics</span></span>
<span data-ttu-id="51ff4-119">Želite li isprobati Microsoft Flow u sustavu SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="51ff4-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="51ff4-120">Stvori tok</span><span class="sxs-lookup"><span data-stu-id="51ff4-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="51ff4-121">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="51ff4-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


