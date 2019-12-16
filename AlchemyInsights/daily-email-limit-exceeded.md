---
title: Prekoračeno je svakodnevno ograničenje e-pošte. Tijek rada je suspendiran.
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053109"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="ce952-103">Dnevna poruka e-pošte premašena.</span><span class="sxs-lookup"><span data-stu-id="ce952-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="ce952-104">Tijek rada je suspendiran.</span><span class="sxs-lookup"><span data-stu-id="ce952-104">Workflow is suspended.</span></span>

<span data-ttu-id="ce952-105">Ova pogreška može se primiti u sljedećim scenarijima:</span><span class="sxs-lookup"><span data-stu-id="ce952-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="ce952-106">Imate tijek rada u SharePoint online koji koristi vrstu platforme SharePoint 2010 ili SharePoint 2013 tijek rada.</span><span class="sxs-lookup"><span data-stu-id="ce952-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="ce952-107">Tijek rada je konfiguriran za slanje prilagođene poruke e-pošte na više od 200 korisnika u isto vrijeme, više od 10.000 primatelja po danu ili više od 30 poruka u minuti.</span><span class="sxs-lookup"><span data-stu-id="ce952-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="ce952-108">Kada pokrenete tijek rada, poruka e-pošte nije poslana i primijetite sljedeće ponašanje:</span><span class="sxs-lookup"><span data-stu-id="ce952-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="ce952-109">Za tijek rada koji koristi vrstu platforme SharePoint 2013, potražite stranicu **status tijeka rada** .</span><span class="sxs-lookup"><span data-stu-id="ce952-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="ce952-110">Na stranici status tijeka rada, **interni status** je postavljen na **pokretanje**, a informativni balon prikazuje **nemogućnost slanja primatelju**.</span><span class="sxs-lookup"><span data-stu-id="ce952-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="ce952-111">Da biste zaobišli taj problem, konfigurirajte tijek rada za slanje poruka e-pošte bez prekoračenja [ograničenja primatelja Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="ce952-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="ce952-112">Na primjer, koristite pauzu u tijeku rada, pošaljite e-poštu u Office 365 grupu, grupu raspodjele ili sigurnosnu grupu koju je omogućila pošta ili poruku pošaljite manje od 200 primatelja odjednom.</span><span class="sxs-lookup"><span data-stu-id="ce952-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="ce952-113">Dodatne informacije potražite u sljedećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="ce952-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="ce952-114">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="ce952-114">Related topics</span></span>
- [<span data-ttu-id="ce952-115">Stvori tok</span><span class="sxs-lookup"><span data-stu-id="ce952-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ce952-116">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="ce952-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 