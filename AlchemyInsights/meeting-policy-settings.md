---
title: Postavke pravilnika za sastanak
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794326"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="e0fdf-102">Upravljanje pravilima sastanka u Microsoftovim timovima</span><span class="sxs-lookup"><span data-stu-id="e0fdf-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="e0fdf-103">**Pažnja: promjenama pravilnika za korisnike može potrajati do 24 sata.**</span><span class="sxs-lookup"><span data-stu-id="e0fdf-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="e0fdf-104">Možda nećete moći odmah unijeti promjene u novostvorenu politiku; Pričekajte 4 sata i pokušajte ponovno izmijeniti novo stvoreno pravilo.</span><span class="sxs-lookup"><span data-stu-id="e0fdf-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="e0fdf-105">Pravila sastanka koriste se za kontrolu značajki dostupnih sudionicima sastanka za sastanke zakazanih od strane korisnika u vašoj tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="e0fdf-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="e0fdf-106">Neke značajke pravilnika za sastanak možda se još ne provode u centru za administratore timova (te su oznake "uskoro" u dokumentaciji).</span><span class="sxs-lookup"><span data-stu-id="e0fdf-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="e0fdf-107">U ovom slučaju ili ako vam se prikazuje pogreška "trenutno ne možemo ažurirati pravilnik, no ponovno je pokušati kasnije" u centru za administratore programa Microsoft timovi preporučujemo da pomoću komponente PowerShell stvorite ili izmijenite pravila sastanka timova.</span><span class="sxs-lookup"><span data-stu-id="e0fdf-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="e0fdf-108">Dodatne informacije o pravilima sastanka potražite u sljedećim resursima:</span><span class="sxs-lookup"><span data-stu-id="e0fdf-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="e0fdf-109">Da biste saznali više o stvaranju pravilnika, promjenama i dodjeljivanju korisnika u pravilnik, pročitajte članak [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="e0fdf-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="e0fdf-110">Da biste promijenili politiku pomoću cmdleta u komponenti PowerShell, pročitajte članak [Prikaz aplikacije PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="e0fdf-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="e0fdf-111">Da biste koristili pravila sastanka za timove, morate koristiti module za sastanke u programu [Skype za tvrtke](https://www.microsoft.com/download/details.aspx?id=39366) .</span><span class="sxs-lookup"><span data-stu-id="e0fdf-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="e0fdf-112">Dodatne informacije potražite u [dokumentaciji za cmdlete \*-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="e0fdf-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

