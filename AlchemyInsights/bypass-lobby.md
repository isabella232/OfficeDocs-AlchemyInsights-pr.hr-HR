---
title: Zaobilaženje predvorja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889074"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="b9fac-102">Kontrolne postavke predvorja i razina sudjelovanja u timovima</span><span class="sxs-lookup"><span data-stu-id="b9fac-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="b9fac-103">Ako želite dopustiti svima, uključujući dial-in, vanjski i anonimni korisnici, **zaobići predvorje**, koristite PowerShell za postizanje ovog zadatka.</span><span class="sxs-lookup"><span data-stu-id="b9fac-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="b9fac-104">Evo primjera izmjene globalne politike sastanka za vašu organizaciju.</span><span class="sxs-lookup"><span data-stu-id="b9fac-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="b9fac-105">Ovaj cmdlet trenutno zahtijeva korištenje Skype za Business PowerShell modul.</span><span class="sxs-lookup"><span data-stu-id="b9fac-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="b9fac-106">Da biste dobili postavljen za korištenje ovog cmdlet, provjerite [Upravljanje pravilima putem PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="b9fac-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="b9fac-107">Nakon što postavite pravilo, morate ga primijeniti na korisnike; ili, ako ste izmijenili globalnu politiku, ona će se automatski odnositi na korisnike.</span><span class="sxs-lookup"><span data-stu-id="b9fac-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="b9fac-108">Za bilo koju promjenu pravila morate pričekati najmanje **4 sata do 24 sata** kako bi pravila stupile na snagu.</span><span class="sxs-lookup"><span data-stu-id="b9fac-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="b9fac-109">Obavezno pregledajte dokumentaciju u nastavku prije nego što učinite te promjene da biste razumjeli što to omogućuje.</span><span class="sxs-lookup"><span data-stu-id="b9fac-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="b9fac-110">Razumijevanje timova za sastanke u predvorju</span><span class="sxs-lookup"><span data-stu-id="b9fac-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="b9fac-111">Ove postavke kontroliraju koji sudionici sastanka čekaju u predvorju prije nego što budu primljeni na sastanak i razini sudjelovanja koje su im dopuštene na sastanku.</span><span class="sxs-lookup"><span data-stu-id="b9fac-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="b9fac-112">Možete koristiti PowerShell da biste ažurirali postavke pravila sastanka koje još nisu provedene (označene "uskoro") u centru za administraciju timova.</span><span class="sxs-lookup"><span data-stu-id="b9fac-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="b9fac-113">Pogledajte u nastavku za primjer PowerShell cmdlet koji omogućuje svim korisnicima da zaobiđu predvorje.</span><span class="sxs-lookup"><span data-stu-id="b9fac-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="b9fac-114">[Automatski priznati](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) da je osoba pravila po organizatoru koja kontrolira hoće li se ljudi izravno pridružiti sastanku ili čekati u predvorju dok ih ne primi autentizirani korisnik.</span><span class="sxs-lookup"><span data-stu-id="b9fac-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="b9fac-115">[Dopusti anonimnim ljudima pokretanje sastanka](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je pravila po organizatoru koja kontrolira mogu li se anonimni ljudi, uključujući B2B i saveznih korisnika, pridružiti sastanku korisnika bez Autenticnog korisnika iz organizacije koja je nazočna.</span><span class="sxs-lookup"><span data-stu-id="b9fac-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="b9fac-116">[Dopustite korisnicima biranja da zaobiđu predvorje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira hoće li se osobe koje telefoniraju telefonom pridružiti sastanku izravno ili čekati u predvorju bez obzira na to jesu li **automatski priznali postavke korisnika** .</span><span class="sxs-lookup"><span data-stu-id="b9fac-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="b9fac-117">[Omogućite organizatori nadjačati postavke predvorja](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira može li organizator sastanka nadjačati postavke predvorja koje je administrator postavio u **automatski priznati ljude** i **dopustiti dial-in korisnicima da zaobiđu predvorje** kada zakazaju novi sastanak.</span><span class="sxs-lookup"><span data-stu-id="b9fac-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="b9fac-118">**Napomena:** Pročitajte [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) za potpuni pregled pravila sastanka Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b9fac-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
