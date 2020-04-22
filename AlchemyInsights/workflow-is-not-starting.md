---
title: Tijek rada se ne pokreće
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766089"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="24b8b-102">Tijek rada se ne pokreće</span><span class="sxs-lookup"><span data-stu-id="24b8b-102">Workflow is not starting</span></span>

- <span data-ttu-id="24b8b-103">Tijekovi rada sustava SharePoint 2010 i SharePoint 2013 ne počinju.</span><span class="sxs-lookup"><span data-stu-id="24b8b-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="24b8b-104">Ako se tijek rada ne pokreće, možda postoji privremeni problem servisa zbog kojeg korisnici mogu naići na povremene odgode s napretkom tijeka rada.</span><span class="sxs-lookup"><span data-stu-id="24b8b-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="24b8b-105">Provjerite [nadzornu ploču stanja servisa](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) da biste provjerili utječe li na vašu tvrtku ili ustanovu.</span><span class="sxs-lookup"><span data-stu-id="24b8b-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="24b8b-106">Ako je prošlo više od 24 sata otkad ste prvi put vidjeli taj problem, prijavite ulaznicu za podršku.</span><span class="sxs-lookup"><span data-stu-id="24b8b-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="24b8b-107">U mnogim slučajevima već radimo na rješenju.</span><span class="sxs-lookup"><span data-stu-id="24b8b-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="24b8b-108">Molimo Vas da nam najmanje 24 sata za dovršetak rješenja.</span><span class="sxs-lookup"><span data-stu-id="24b8b-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="24b8b-109">Tijekovi rada sustava SharePoint 2010 odgođeni su pri pokretanju.</span><span class="sxs-lookup"><span data-stu-id="24b8b-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="24b8b-110">To se događa ako se tijek rada pokreće u velikim serijama.</span><span class="sxs-lookup"><span data-stu-id="24b8b-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="24b8b-111">(na primjer, kada se dodaje nekoliko stavki odjednom).</span><span class="sxs-lookup"><span data-stu-id="24b8b-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="24b8b-112">Tijekovi rada nisu dizajnirani za pokretanje u stvarnom vremenu, stoga je kašnjenje ponašanje po dizajnu.</span><span class="sxs-lookup"><span data-stu-id="24b8b-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="24b8b-113">Ako je tijek rada složen Extensible Object Markup Language (XMOL), kompilacija može biti spora.</span><span class="sxs-lookup"><span data-stu-id="24b8b-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="24b8b-114">Provjerite [ovaj](https://support.microsoft.com//kb/3043697) članak.</span><span class="sxs-lookup"><span data-stu-id="24b8b-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="24b8b-115">Trebali biste pojednostaviti tijek rada ili ga redizajnirati pomoću vrste platforme Tijek rada sustava Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="24b8b-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="24b8b-116">Ako je povijest tijeka rada narasla, možda želite očistiti stavke ili stvoriti novi popis povijesti.</span><span class="sxs-lookup"><span data-stu-id="24b8b-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="24b8b-117">Dodatne informacije : [Čišćenje povijesti tijeka rada](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="24b8b-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="24b8b-118">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="24b8b-118">Related topics</span></span>
<span data-ttu-id="24b8b-119">Želite li isprobati Microsoft Flow u sustavu SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="24b8b-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="24b8b-120">Stvori tijek</span><span class="sxs-lookup"><span data-stu-id="24b8b-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="24b8b-121">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="24b8b-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


