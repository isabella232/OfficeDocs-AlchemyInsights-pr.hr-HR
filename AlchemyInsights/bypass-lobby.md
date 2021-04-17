---
title: Zaobilazno predvorje
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820026"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="7cf7d-102">Upravljanje postavkama predvorja i razinom sudjelovanja u aplikaciji Teams</span><span class="sxs-lookup"><span data-stu-id="7cf7d-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="7cf7d-103">Ako želite omogućiti svima, uključujući uključivanje biranjem, vanjske i anonimne korisnike, da zaobilaze predvorje, upotrijebite PowerShell da biste izvršili taj zadatak.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="7cf7d-104">Evo primjera izmjene pravilnika globalnog sastanka za vašu organizaciju.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="7cf7d-105">Ovaj cmdlet trenutno zahtijeva korištenje modula PowerShell skypea za tvrtke.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="7cf7d-106">Da biste se postavili za korištenje ovog cmdleta, pogledajte upravljanje [pravilnikom putem komponente PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="7cf7d-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="7cf7d-107">Kada postavite pravilnik, morate ga primijeniti na korisnike. ili, ako ste izmijenili globalni pravilnik, on će se automatski primijeniti na korisnike.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="7cf7d-108">Da bi se pravila mijenjala, morate pričekati najmanje **4 sata do 24 sata da** bi pravila snazi.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="7cf7d-109">Obavezno pregledajte dokumentaciju u nastavku da biste točno razumjeli što to omogućuje.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="7cf7d-110">Objašnjenje kontrola pravilnika u predvorju sastanka u aplikaciji Teams</span><span class="sxs-lookup"><span data-stu-id="7cf7d-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="7cf7d-111">Te postavke kontroliraju sudionike sastanka koji čekaju u predvorju prije nego što se prihvate na sastanak i razinu sudjelovanja koja im je dopuštena u sastanku.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="7cf7d-112">PowerShell možete koristiti za ažuriranje postavki pravilnika sastanka koje još nisu implementirane (označene kao "uskoro") u centru za administratore aplikacije Teams.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="7cf7d-113">U nastavku pogledajte primjer cmdleta Komponente PowerShell koji svim korisnicima omogućuje zaobilaženje predvorja.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="7cf7d-114">[Automatsko priznanje osoba](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) pravilnik je po organizatoru koji određuje hoće li se osobe izravno uključiti u sastanak ili čekati u predvorju dok ih korisnik ne primi.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="7cf7d-115">[Omogući anonimnim osobama](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) da započinju sastanak pravilnik je po organizatoru koji određuje mogu li se anonimne osobe, uključujući B2B i združene korisnike, uključiti u korisnikov sastanak bez provjere autentičnosti korisnika iz tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="7cf7d-116">[Omogući korisnicima uključivanje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) biranjem da zaobilaze predvorje **(uskoro**) pravilnik je po organizatoru koji određuje hoće li se osobe koje se pozivaju telefonom izravno uključiti u sastanak ili čekati u predvorju bez obzira na postavku Automatski **priznaj osobe.**</span><span class="sxs-lookup"><span data-stu-id="7cf7d-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="7cf7d-117">[Dopusti organizatorima da nadjačaju](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) postavke predvorja (uskoro ) pravilnik je po organizatoru koji  određuje može li organizator sastanka nadjačati postavke predvorja koje je postavio administrator u odjeljku Automatski prima osobe i Dopusti korisnicima za uključivanje **biranjem** da zaobilaze predvorje kada zakaže novi sastanak.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="7cf7d-118">**Napomena:** Pročitajte [članak Upravljanje pravilnikom za sastanke u aplikaciji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) da biste pregledali pravilnike za sastanke aplikacije Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7cf7d-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
