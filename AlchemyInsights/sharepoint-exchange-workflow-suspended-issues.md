---
title: Početak rada sa sustavom SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051633"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="63512-102">Tijekovi rada u sustavu SharePoint</span><span class="sxs-lookup"><span data-stu-id="63512-102">Workflows in SharePoint</span></span>

<span data-ttu-id="63512-103">Ako tijekovi rada sustava SharePoint ne šalju e-poštu, vaša je organizacija možda naišla na ograničenja pošiljatelja sustava Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="63512-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="63512-104">Poruka o pogrešci "tijek rada je suspendirana" može se pojaviti ako imate jednu od sljedećih stavki:</span><span class="sxs-lookup"><span data-stu-id="63512-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="63512-105">Imate tijek rada u SharePoint online koji koristi vrstu platforme SharePoint 2010 ili SharePoint 2013 tijek rada.</span><span class="sxs-lookup"><span data-stu-id="63512-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="63512-106">Tijek rada je konfiguriran za slanje prilagođene poruke e-pošte na više od 200 korisnika u isto vrijeme, više od 10.000 primatelja po danu ili više od 30 poruka u minuti.</span><span class="sxs-lookup"><span data-stu-id="63512-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="63512-107">Kada pokrenete tijek rada, poruka e-pošte nije poslana i primijetite poruku o pogrešci, interni status je postavljen na suspendirano ili nije moguće poslati primatelju.</span><span class="sxs-lookup"><span data-stu-id="63512-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="63512-108">Za više informacija, molimo pogledajte sljedeći [članak](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="63512-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

