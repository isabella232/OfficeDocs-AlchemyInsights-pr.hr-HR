---
title: Postavke pravilnika sastanka
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825435"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="d6327-102">Upravljanje pravilima sastanka u aplikaciji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d6327-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="d6327-103">**Napomena: korisnicima može trebati do 24 sata da promjene pravilnika stupe na snagu.**</span><span class="sxs-lookup"><span data-stu-id="d6327-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="d6327-104">Možda nećete moći odmah mijenjati novostvorene pravilnike. pričekajte 4 sata i pokušajte ponovno izmijeniti novostvoreni pravilnik.</span><span class="sxs-lookup"><span data-stu-id="d6327-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="d6327-105">Pravila sastanka koriste se za kontrolu značajki koje su dostupne sudionicima sastanka za sastanke koje zakazali korisnici u vašoj tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="d6327-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="d6327-106">Neke značajke pravilnika za sastanke možda se još neće implementirati u centru za administratore aplikacije Teams (one su u dokumentaciji označene kao "uskoro").</span><span class="sxs-lookup"><span data-stu-id="d6327-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="d6327-107">U tom slučaju ili ako vam se prikazuje pogreška kao što je "Trenutno ne možemo ažurirati pravilnik, ali ga kasnije pokušati ponovno" u centru za administratore aplikacije Microsoft Teams, preporučujemo da pomoću komponente PowerShell stvorite ili izmijenite pravilnike za sastanke servisa Teams.</span><span class="sxs-lookup"><span data-stu-id="d6327-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="d6327-108">Dodatne informacije o pravilima sastanka potražite u sljedećim resursima:</span><span class="sxs-lookup"><span data-stu-id="d6327-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="d6327-109">Informacije o stvaranju pravilnika, unošanju promjena i dodjeljivanju korisnika pravilniku pogledajte u članku Upravljanje [pravilnikom za sastanke u aplikaciji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="d6327-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="d6327-110">Da biste unijeli promjene pravilnika pomoću cmdleta komponente PowerShell, pogledajte [pregled komponente Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="d6327-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="d6327-111">Morate koristiti modul [PowerShell skypea za tvrtke za pravilnike](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) sastanka aplikacije Teams.</span><span class="sxs-lookup"><span data-stu-id="d6327-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="d6327-112">Dodatne informacije [potražite u dokumentaciji cmdleta \*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="d6327-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

