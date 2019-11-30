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
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627566"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="d5acd-102">Upravljanje pravilima sastanka u Microsoftovim timovima</span><span class="sxs-lookup"><span data-stu-id="d5acd-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="d5acd-103">Pravila sastanka koriste se za kontrolu značajki koje su dostupne sudionicima koji ispunjavaju sastanke koje su zakazali korisnici u vašoj organizaciji.</span><span class="sxs-lookup"><span data-stu-id="d5acd-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="d5acd-104">Neke značajke politika sastanka možda neće biti implementirane u centru za administraciju timova još uvijek (oni su označeni "uskoro" u dokumentaciji).</span><span class="sxs-lookup"><span data-stu-id="d5acd-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="d5acd-105">U tom slučaju, ili ako ste uzimajući pogrešku kao što je "ne možemo ažurirati pravila upravo sada, ali pokušajte ponovno kasnije" u Microsoft Teams centar za administraciju, preporučujemo da koristite PowerShell za stvaranje ili izmjenu pravila sastanka timova.</span><span class="sxs-lookup"><span data-stu-id="d5acd-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="d5acd-106">Dodatne informacije o pravilima sastanka potražite u sljedećim resursima:</span><span class="sxs-lookup"><span data-stu-id="d5acd-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="d5acd-107">Da biste saznali više o stvaranju pravila, stvaranju promjena i dodjeljivanju korisnika pravilima, pogledajte [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="d5acd-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="d5acd-108">Da biste napravili promjene pravila pomoću PowerShell cmdlets, pogledajte [timove PowerShell pregled](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="d5acd-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="d5acd-109">Morate koristiti [modul Skype za tvrtke PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) za pravila sastanka timova.</span><span class="sxs-lookup"><span data-stu-id="d5acd-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="d5acd-110">Pregled [\*-csteamsmetingpolicy dokumente Cmdletovi](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) za više informacija.</span><span class="sxs-lookup"><span data-stu-id="d5acd-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="d5acd-111">**Napomena:** Može potrajati i do 24 sata da bi promjene politike stupile na snagu za korisnike.</span><span class="sxs-lookup"><span data-stu-id="d5acd-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="d5acd-112">Možda nećete moći odmah mijenjati novostvorene politike; čekati 4 sata i ponovno pokušati izmijeniti novostvorena pravila.</span><span class="sxs-lookup"><span data-stu-id="d5acd-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="d5acd-113">Ako još uvijek imate problema, pokušajte PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d5acd-113">If you're still having problems, try PowerShell.</span></span>  