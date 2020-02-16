---
title: Postavke pravila sastanka
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042836"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="b2286-102">Upravljanje pravilima sastanka u microsoft teams</span><span class="sxs-lookup"><span data-stu-id="b2286-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="b2286-103">**Napomena: može potrajati i do 24 sata da promjene pravila stupe na snagu za korisnike.**</span><span class="sxs-lookup"><span data-stu-id="b2286-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="b2286-104">Možda nećete moći odmah izmijeniti novostvorena pravila; pričekajte 4 sata i pokušajte ponovno izmijeniti novostvorena pravila.</span><span class="sxs-lookup"><span data-stu-id="b2286-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="b2286-105">Pravila sastanka koriste se za kontrolu značajki dostupnih sudionicima sastanka za sastanke koje su zakazali korisnici u vašoj tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="b2286-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="b2286-106">Neke značajke pravila sastanka možda se još neće implementirati u centru za administratore sustava Teams (one su uskoro označene kao "uskoro" u dokumentaciji).</span><span class="sxs-lookup"><span data-stu-id="b2286-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="b2286-107">U tom slučaju ili ako vam se prikaže pogreška kao što je "Ne možemo ažurirati pravila odmah, ali pokušajte ponovno kasnije" u centru za administratore sustava Microsoft Teams, preporučujemo da koristite PowerShell za stvaranje ili izmjenu pravila sastanka sustava Teams.</span><span class="sxs-lookup"><span data-stu-id="b2286-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="b2286-108">Dodatne informacije o pravilima sastanka potražite u sljedećim resursima:</span><span class="sxs-lookup"><span data-stu-id="b2286-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="b2286-109">Da biste saznali više o stvaranju pravila, unosenju promjena i dodjeli korisnika pravilima, pročitajte odjeljko [Upravljanje pravilima sastanka u sustavu Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="b2286-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="b2286-110">Da biste promijenili pravila pomoću cmdleta komponente PowerShell, pogledajte [pregled komponente Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="b2286-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="b2286-111">Morate koristiti [modul PowerShell servisa Skype za tvrtke](https://www.microsoft.com/download/details.aspx?id=39366) za pravilniko o sastanku sustava Teams.</span><span class="sxs-lookup"><span data-stu-id="b2286-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="b2286-112">Dodatne informacije potražite u [dokumentaciji cmdleta \*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="b2286-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

