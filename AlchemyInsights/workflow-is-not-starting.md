---
title: Tijek rada se ne započinje
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738081"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="12ad6-102">Tijek rada se ne započinje</span><span class="sxs-lookup"><span data-stu-id="12ad6-102">Workflow is not starting</span></span>

- <span data-ttu-id="12ad6-103">Tijekovi rada sustava SharePoint 2010 i SharePoint 2013 se ne počinju.</span><span class="sxs-lookup"><span data-stu-id="12ad6-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="12ad6-104">Ako se tijek rada ne započinje, možda postoji problem s privremenim servisima u kojem korisnici mogu doživjeti povremene odgode s napretkom tijeka rada.</span><span class="sxs-lookup"><span data-stu-id="12ad6-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="12ad6-105">Provjerite je li vaša tvrtka ili ustanova utjecala na [nadzornu ploču za zdravstvenu službu](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) .</span><span class="sxs-lookup"><span data-stu-id="12ad6-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="12ad6-106">Ako je prošlo više od 24 sata od kada ste prvi put vidjeli ovaj problem, molimo prijavite ulaznicu za podršku.</span><span class="sxs-lookup"><span data-stu-id="12ad6-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="12ad6-107">U mnogim slučajevima već radimo na rješenju.</span><span class="sxs-lookup"><span data-stu-id="12ad6-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="12ad6-108">Molim vas, dajte nam najmanje 24 sata da dovršimo rješenje.</span><span class="sxs-lookup"><span data-stu-id="12ad6-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="12ad6-109">Tijekovi rada sustava SharePoint 2010 odgođeni na početku.</span><span class="sxs-lookup"><span data-stu-id="12ad6-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="12ad6-110">To se događa ako se tijek rada aktivira u velikim serijama.</span><span class="sxs-lookup"><span data-stu-id="12ad6-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="12ad6-111">(na primjer, kada se nekoliko stavki doda odjednom).</span><span class="sxs-lookup"><span data-stu-id="12ad6-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="12ad6-112">Tijekovi rada nisu dizajnirani za izvođenje u realnom vremenu, tako da je odgoda po dizajnu ponašanje.</span><span class="sxs-lookup"><span data-stu-id="12ad6-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="12ad6-113">Ako je tijek rada složen Extensible Object Markup Language (XMOL), kompilacija može biti spora.</span><span class="sxs-lookup"><span data-stu-id="12ad6-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="12ad6-114">Provjerite [ovaj](https://support.microsoft.com//kb/3043697) članak.</span><span class="sxs-lookup"><span data-stu-id="12ad6-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="12ad6-115">Trebali biste pojednostavniti tijek rada ili ga redizajnirati pomoću vrste platforme Microsoft SharePoint 2013 workflow.</span><span class="sxs-lookup"><span data-stu-id="12ad6-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="12ad6-116">Ako je vaša povijest tijeka rada narasla, možda želite očistiti stavke ili stvoriti novi popis povijesti.</span><span class="sxs-lookup"><span data-stu-id="12ad6-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="12ad6-117">Dodatne informacije: [čišćenje povijesti tijeka rada](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="12ad6-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="12ad6-118">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="12ad6-118">Related topics</span></span>
<span data-ttu-id="12ad6-119">Želite li isprobati Microsoft Flow u sustavu SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="12ad6-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="12ad6-120">Stvori tok</span><span class="sxs-lookup"><span data-stu-id="12ad6-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="12ad6-121">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="12ad6-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


