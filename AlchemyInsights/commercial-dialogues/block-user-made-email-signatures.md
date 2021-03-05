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
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481205"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="798dd-102">Blokiranje korisničkog potpisa e-pošte</span><span class="sxs-lookup"><span data-stu-id="798dd-102">Block user-made email signatures</span></span>

<span data-ttu-id="798dd-103">Sljedeće rješenje primjenjuje se samo na potpise e-pošte stvorene u programu Outlook na webu.</span><span class="sxs-lookup"><span data-stu-id="798dd-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="798dd-104">Potpise možete blokirati samo u aplikaciji Outlook ako imate lokalni poslužitelj sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="798dd-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="798dd-105">U centru za administratore odaberite **Exchange centri za administratore**  >  .</span><span class="sxs-lookup"><span data-stu-id="798dd-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="798dd-106">Kliknite **dozvole** za  >  **Outlook Web App**.</span><span class="sxs-lookup"><span data-stu-id="798dd-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="798dd-107">Odaberite pravilo, a zatim kliknite ikonu olovke da biste je uredili.</span><span class="sxs-lookup"><span data-stu-id="798dd-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="798dd-108">Kliknite **značajke**  >  **više mogućnosti**.</span><span class="sxs-lookup"><span data-stu-id="798dd-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="798dd-109">U odjeljku **korisničko iskustvo** poništite potvrdni okvir **potpis e-pošte** , a zatim kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="798dd-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="798dd-110">**Važno:** Ako je potpis dodan prije nego što poništite taj potvrdni okvir, korisnik će ga i dalje moći koristiti.</span><span class="sxs-lookup"><span data-stu-id="798dd-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="798dd-111">Zamolite ih da ga uklanjaju.</span><span class="sxs-lookup"><span data-stu-id="798dd-111">Ask them to remove it.</span></span>
