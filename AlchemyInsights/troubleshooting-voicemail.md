---
title: 'Poruka o otklanjanju poteškoća '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677017"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="2f6c8-102">Poruka o otklanjanju poteškoća</span><span class="sxs-lookup"><span data-stu-id="2f6c8-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="2f6c8-103">Provjerite je li značajka zauzetosti na zaposlenom namjerna.</span><span class="sxs-lookup"><span data-stu-id="2f6c8-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="2f6c8-104">Ako ta značajka nije potrebna na ovom korisniku:</span><span class="sxs-lookup"><span data-stu-id="2f6c8-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="2f6c8-105">Otvorite [centar za administratore timova](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="2f6c8-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="2f6c8-106">Na lijevoj traci Navigirajte **govorna**  >  **pravila** za  >  **Upravljanje pravilima** za **pravilnik o pozivu**.</span><span class="sxs-lookup"><span data-stu-id="2f6c8-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="2f6c8-107">Odaberite **Upravljanje korisnicima**.</span><span class="sxs-lookup"><span data-stu-id="2f6c8-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="2f6c8-108">Potražite korisnika i promijenite pravilnik poziva u neku koja ima **zauzetosti na zauzetosti dostupna je kada ste u pozivu** na **Isključeno**.</span><span class="sxs-lookup"><span data-stu-id="2f6c8-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="2f6c8-109">Kliknite **Primijeni**.</span><span class="sxs-lookup"><span data-stu-id="2f6c8-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="2f6c8-110">Promjena pravilnika može potrajati i do 24 sata da bi se replicirali.</span><span class="sxs-lookup"><span data-stu-id="2f6c8-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="2f6c8-111">Dodatne informacije o toj značajki upućuju na: [zauzeto na zauzeto dostupno je tijekom poziva](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="2f6c8-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
