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
ms.openlocfilehash: 5ee77e57b3bc64d7a04256ab67b691e5205eac56
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626340"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="9609c-102">Kontrolne postavke predvorja i razina sudjelovanja</span><span class="sxs-lookup"><span data-stu-id="9609c-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="9609c-103">Ako želite dopustiti svima, uključujući dial-in, vanjski i anonimni korisnici zaobići predvorje u Microsoft Teams, možete koristiti PowerShell za to.</span><span class="sxs-lookup"><span data-stu-id="9609c-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="9609c-104">Evo primjera izmjene globalne politike sastanka za vašu organizaciju:</span><span class="sxs-lookup"><span data-stu-id="9609c-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="9609c-105">Ovaj cmdlet trenutno zahtijeva korištenje Skype za Business PowerShell modul.</span><span class="sxs-lookup"><span data-stu-id="9609c-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="9609c-106">Da biste dobili setup koristiti ovaj cmdlet, provjerite [Upravljanje pravilima putem PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="9609c-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="9609c-107">Možete postaviti novo pravilo koje ćete zatim morati primijeniti na korisnike.</span><span class="sxs-lookup"><span data-stu-id="9609c-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="9609c-108">Ako izmijenite globalnu politiku, ona će se automatski odnositi na korisnike.</span><span class="sxs-lookup"><span data-stu-id="9609c-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="9609c-109">Za bilo koju promjenu pravila morate pričekati najmanje 4 sata i do 24 sata kako bi pravila stupile na snagu.</span><span class="sxs-lookup"><span data-stu-id="9609c-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="9609c-110">Obavezno pregledajte dokumentaciju u nastavku prije nego što učinite te promjene da biste razumjeli što to omogućuje.</span><span class="sxs-lookup"><span data-stu-id="9609c-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="9609c-111">Razumijevanje timova za sastanke u predvorju</span><span class="sxs-lookup"><span data-stu-id="9609c-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="9609c-112">[Automatski priznati](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) da je osoba pravila po organizatoru koja kontrolira hoće li se ljudi izravno pridružiti sastanku ili čekati u predvorju dok ih ne primi autentizirani korisnik.</span><span class="sxs-lookup"><span data-stu-id="9609c-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="9609c-113">[Dopusti anonimnim ljudima pokretanje sastanka](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je pravila po organizatoru koja kontrolira mogu li se anonimni ljudi, uključujući B2B i saveznih korisnika, pridružiti sastanku korisnika bez Autenticnog korisnika iz organizacije koja je nazočna.</span><span class="sxs-lookup"><span data-stu-id="9609c-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="9609c-114">[Dopustite korisnicima biranja da zaobiđu predvorje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira hoće li se osobe koje telefoniraju telefonom pridružiti sastanku izravno ili čekati u predvorju bez obzira na to jesu li **automatski priznali postavke korisnika** .</span><span class="sxs-lookup"><span data-stu-id="9609c-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="9609c-115">[Omogućite organizatori nadjačati postavke predvorja](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira može li organizator sastanka nadjačati postavke predvorja koje je administrator postavio u **automatski priznati ljude** i **dopustiti dial-in korisnicima da zaobiđu predvorje** kada zakazaju novi sastanak.</span><span class="sxs-lookup"><span data-stu-id="9609c-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="9609c-116">**Napomena:** Pročitajte [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) za potpuni pregled pravila sastanka Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9609c-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
