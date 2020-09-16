---
title: Prekoračena je dnevna ograničenje e-pošte. Tijek rada je obustavljen.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731555"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="a667f-103">Prekoračena je dnevna ograničenje e-pošte.</span><span class="sxs-lookup"><span data-stu-id="a667f-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="a667f-104">Tijek rada je obustavljen.</span><span class="sxs-lookup"><span data-stu-id="a667f-104">Workflow is suspended.</span></span>

<span data-ttu-id="a667f-105">Ta se pogreška može primiti u sljedećim scenarijima:</span><span class="sxs-lookup"><span data-stu-id="a667f-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="a667f-106">Imate tijek rada u sustavu SharePoint online koji koristi vrstu platforme tijeka rada sustava SharePoint 2010 ili SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="a667f-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="a667f-107">Tijek rada konfiguriran je za slanje prilagođene poruke e-pošte na više od 200 korisnika istodobno, više od 10.000 primatelja dnevno ili više od 30 poruka po minuti.</span><span class="sxs-lookup"><span data-stu-id="a667f-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="a667f-108">Kada pokrenete tijek rada, poruka e-pošte ne šalje se i primijetit ćete sljedeće ponašanje:</span><span class="sxs-lookup"><span data-stu-id="a667f-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="a667f-109">Za tijek rada pomoću vrste platforme sustava SharePoint 2013 možete potražiti stranicu **statusa tijeka rada** .</span><span class="sxs-lookup"><span data-stu-id="a667f-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="a667f-110">Na stranici Stanje tijeka rada, **interni status** postavljen je na **pokrenut**, a balon informacija **ne može se prikazati primatelju**.</span><span class="sxs-lookup"><span data-stu-id="a667f-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="a667f-111">Da biste zaobišli taj problem, konfigurirajte tijek rada za slanje poruka e-pošte bez prekoračenja [ograničenja pošiljatelja sustava Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="a667f-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="a667f-112">Na primjer, koristite pauzu u tijeku rada, pošaljite poruku e-pošte grupi Microsoft 365, grupi za raspodjelu ili sigurnosnoj grupi za e-poštu ili pošaljite poruku na manje od 200 primatelja istodobno.</span><span class="sxs-lookup"><span data-stu-id="a667f-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="a667f-113">Dodatne informacije potražite u sljedećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="a667f-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="a667f-114">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="a667f-114">Related topics</span></span>
- [<span data-ttu-id="a667f-115">Stvaranje toka</span><span class="sxs-lookup"><span data-stu-id="a667f-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a667f-116">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="a667f-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 