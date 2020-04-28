---
title: Premašeno je dnevno ograničenje e-pošte. Tijek rada je obustavljen.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908696"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="ef918-103">Premašilo je dnevno ograničenje e-pošte.</span><span class="sxs-lookup"><span data-stu-id="ef918-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="ef918-104">Tijek rada je obustavljen.</span><span class="sxs-lookup"><span data-stu-id="ef918-104">Workflow is suspended.</span></span>

<span data-ttu-id="ef918-105">Ova pogreška može se primiti u sljedećim scenarijima:</span><span class="sxs-lookup"><span data-stu-id="ef918-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="ef918-106">Imate tijek rada u sustavu SharePoint Online koji koristi vrstu platforme tijeka rada sustava SharePoint 2010 ili SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="ef918-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="ef918-107">Tijek rada konfiguriran je za slanje prilagođene poruke e-pošte većem broju od 200 korisnika odjednom, više od 10 000 primatelja dnevno ili više od 30 poruka u minuti.</span><span class="sxs-lookup"><span data-stu-id="ef918-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="ef918-108">Kada pokrenete tijek rada, poruka e-pošte se ne šalje i primijetite sljedeće ponašanje:</span><span class="sxs-lookup"><span data-stu-id="ef918-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="ef918-109">Za tijek rada koji koristi vrstu platforme Sustava SharePoint 2013 potražite stranicu **Stanja tijeka rada.**</span><span class="sxs-lookup"><span data-stu-id="ef918-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="ef918-110">Na stranici Stanja tijeka rada **interno je stanje** postavljeno na **Pokrenuto**, a oblačić s informacijama prikazuje **nije moguće poslati primatelju**.</span><span class="sxs-lookup"><span data-stu-id="ef918-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="ef918-111">Da biste zaobišli taj problem, konfigurirajte tijek rada za slanje poruka e-pošte bez prekoračenja [ograničenja pošiljatelja sustava Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="ef918-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="ef918-112">Na primjer, koristite pauzu u tijeku rada, pošaljite e-poštu grupi microsoft 365, grupi za raspodjelu ili sigurnosnoj grupi omogućenoj za poštu ili pošaljite poruku manje od 200 primatelja odjednom.</span><span class="sxs-lookup"><span data-stu-id="ef918-112">For example, use a pause in the workflow, send the email to an Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="ef918-113">Dodatne informacije potražite u sljedećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="ef918-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="ef918-114">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="ef918-114">Related topics</span></span>
- [<span data-ttu-id="ef918-115">Stvori tijek</span><span class="sxs-lookup"><span data-stu-id="ef918-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ef918-116">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="ef918-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 