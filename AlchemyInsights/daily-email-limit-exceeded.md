---
title: Premašeno je dnevno ograničenje e-pošte. Tijek rada obustavljen.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514435"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="bc3a3-103">Dnevni e-pošta Premašeno ograničenje.</span><span class="sxs-lookup"><span data-stu-id="bc3a3-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="bc3a3-104">Tijek rada obustavljen.</span><span class="sxs-lookup"><span data-stu-id="bc3a3-104">Workflow is suspended.</span></span>

<span data-ttu-id="bc3a3-105">Ova se pogreška možda primili u sljedećim scenarijima:</span><span class="sxs-lookup"><span data-stu-id="bc3a3-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="bc3a3-106">Imate tijeka rada u SharePoint Online koji koriste SharePoint 2010 ili vrsta platformi SharePoint 2013 tijeka rada.</span><span class="sxs-lookup"><span data-stu-id="bc3a3-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="bc3a3-107">Tijek rada konfiguriran za slanje poruka e-pošte prilagođenih više od 200 korisnicima na vrijeme, više od 10 000 primatelja po danu ili na više od 30 poruka u minuti.</span><span class="sxs-lookup"><span data-stu-id="bc3a3-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="bc3a3-108">Kada pokrenete tijek rada, poruka e-pošte nije poslana i primijetiti sljedeće ponašanje:</span><span class="sxs-lookup"><span data-stu-id="bc3a3-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="bc3a3-109">Za tijek rada pomoću vrsta platformi SharePoint 2013 pregledavati stranicu **Stanje tijeka rada** .</span><span class="sxs-lookup"><span data-stu-id="bc3a3-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="bc3a3-110">Na stranici Stanje tijeka rada **Interna Status** postavljen u **pokrenuto**i prikazuje balončić informacije **nije bilo moguće poslati primatelju**.</span><span class="sxs-lookup"><span data-stu-id="bc3a3-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="bc3a3-111">Da biste zaobišli taj problem, konfigurirajte tijeka rada za slanje poruka e-pošte bez Prekoračenje [ograničenja Exchange Online pošiljatelja](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="bc3a3-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="bc3a3-112">Ako, na primjer, koristiti zaustavljanje u tijeku rada, slanje e-pošte grupi Office 365, grupu raspodjele ili pošte omogućeno sigurnosne grupe ili poslati poruku manje od 200 primateljima odjednom.</span><span class="sxs-lookup"><span data-stu-id="bc3a3-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="bc3a3-113">Za dodatne informacije pogledajte sljedeći [članak](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="bc3a3-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="bc3a3-114">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="bc3a3-114">Related topics</span></span>
- [<span data-ttu-id="bc3a3-115">Stvaranje toka</span><span class="sxs-lookup"><span data-stu-id="bc3a3-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="bc3a3-116">SharePoint i tijek</span><span class="sxs-lookup"><span data-stu-id="bc3a3-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 