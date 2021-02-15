---
title: Blokiranje korisničkog potpisa e-pošte
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243263"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="49ec5-102">Blokiranje korisničkog potpisa e-pošte</span><span class="sxs-lookup"><span data-stu-id="49ec5-102">Block user-made email signatures</span></span>

<span data-ttu-id="49ec5-103">Sljedeće rješenje primjenjuje se samo na potpise e-pošte stvorene u programu Outlook na webu.</span><span class="sxs-lookup"><span data-stu-id="49ec5-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="49ec5-104">Potpise možete blokirati samo u aplikaciji Outlook ako imate lokalni poslužitelj sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="49ec5-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="49ec5-105">U centru za administratore odaberite **Exchange centri za administratore**  >  .</span><span class="sxs-lookup"><span data-stu-id="49ec5-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="49ec5-106">Kliknite **dozvole** za  >  **Outlook Web App**.</span><span class="sxs-lookup"><span data-stu-id="49ec5-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="49ec5-107">Odaberite pravilo, a zatim kliknite ikonu olovke da biste je uredili.</span><span class="sxs-lookup"><span data-stu-id="49ec5-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="49ec5-108">Kliknite **značajke**  >  **više mogućnosti**.</span><span class="sxs-lookup"><span data-stu-id="49ec5-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="49ec5-109">U odjeljku **korisničko iskustvo** poništite potvrdni okvir **potpis e-pošte** , a zatim kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="49ec5-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="49ec5-110">**Važno:** Ako je potpis dodan prije nego što poništite taj potvrdni okvir, korisnik će ga i dalje moći koristiti.</span><span class="sxs-lookup"><span data-stu-id="49ec5-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="49ec5-111">Zamolite ih da ga uklanjaju.</span><span class="sxs-lookup"><span data-stu-id="49ec5-111">Ask them to remove it.</span></span>
