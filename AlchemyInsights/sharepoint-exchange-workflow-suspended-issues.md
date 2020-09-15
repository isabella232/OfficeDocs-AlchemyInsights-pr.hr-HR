---
title: Početak rada sa sustavom SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700699"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="9b43e-102">Tijekovi rada u sustavu SharePoint</span><span class="sxs-lookup"><span data-stu-id="9b43e-102">Workflows in SharePoint</span></span>

<span data-ttu-id="9b43e-103">Ako tijekovi rada sustava SharePoint ne šalju poruke e-pošte, vaša je tvrtka ili ustanova mogla naići na ograničenja pošiljatelja sustava Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="9b43e-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="9b43e-104">Poruka o pogrešci "tijek rada se obustavljena" može se pojaviti ako imate neku od sljedećih stavki:</span><span class="sxs-lookup"><span data-stu-id="9b43e-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="9b43e-105">Imate tijek rada u sustavu SharePoint online koji koristi vrstu platforme tijeka rada sustava SharePoint 2010 ili SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="9b43e-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="9b43e-106">Tijek rada konfiguriran je za slanje prilagođene poruke e-pošte na više od 200 korisnika istodobno, više od 10.000 primatelja dnevno ili više od 30 poruka po minuti.</span><span class="sxs-lookup"><span data-stu-id="9b43e-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="9b43e-107">Kada pokrenete tijek rada, poruka e-pošte nije poslana i primijetit ćete poruku o pogrešci, interni je status postavljen na obustavljeno ili nije moguće poslati primatelju.</span><span class="sxs-lookup"><span data-stu-id="9b43e-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="9b43e-108">Dodatne informacije potražite u sljedećem [članku](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="9b43e-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

