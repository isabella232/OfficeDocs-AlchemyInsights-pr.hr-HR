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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376561"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="ae36d-102">Kontrolne postavke predvorja i razina sudjelovanja</span><span class="sxs-lookup"><span data-stu-id="ae36d-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="ae36d-103">Ove postavke kontroliraju koji sudionici sastanka čekaju u predvorju prije nego što budu primljeni na sastanak i razini sudjelovanja koje su im dopuštene na sastanku.</span><span class="sxs-lookup"><span data-stu-id="ae36d-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="ae36d-104">Možete koristiti PowerShell da biste ažurirali postavke pravila sastanka koje još nisu provedene (označene "uskoro") u centru za administraciju timova.</span><span class="sxs-lookup"><span data-stu-id="ae36d-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="ae36d-105">Pogledajte u nastavku za primjer PowerShell cmdlet koji omogućuje svim korisnicima da zaobiđu predvorje.</span><span class="sxs-lookup"><span data-stu-id="ae36d-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="ae36d-106">[Automatski priznati](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) da je osoba pravila po organizatoru koja kontrolira hoće li se ljudi izravno pridružiti sastanku ili čekati u predvorju dok ih ne primi autentizirani korisnik.</span><span class="sxs-lookup"><span data-stu-id="ae36d-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="ae36d-107">[Dopusti anonimnim ljudima pokretanje sastanka](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je pravila po organizatoru koja kontrolira mogu li se anonimni ljudi, uključujući B2B i saveznih korisnika, pridružiti sastanku korisnika bez Autenticnog korisnika iz organizacije koja je nazočna.</span><span class="sxs-lookup"><span data-stu-id="ae36d-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="ae36d-108">[Dopustite korisnicima biranja da zaobiđu predvorje](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira hoće li se osobe koje telefoniraju telefonom pridružiti sastanku izravno ili čekati u predvorju bez obzira na to jesu li **automatski priznali postavke korisnika** .</span><span class="sxs-lookup"><span data-stu-id="ae36d-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="ae36d-109">[Omogućite organizatori premostiti postavke predvorja](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira može li organizator sastanka nadjačati postavke predvorja koje je administrator postavio u **automatski priznati osobe** i **dopustiti biranje korisnike da zaobiđu predvorje** kada zakazaju novi sastanak.</span><span class="sxs-lookup"><span data-stu-id="ae36d-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="ae36d-110">**Napomena:** Pročitajte [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) za potpuni pregled pravila sastanka Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ae36d-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="ae36d-111">**Primjer PowerShell**</span><span class="sxs-lookup"><span data-stu-id="ae36d-111">**PowerShell example**</span></span>

<span data-ttu-id="ae36d-112">Ako želite dopustiti svima, uključujući vanjske ili anonimne korisnike, zaobići predvorje, također možete koristiti PowerShell za postizanje ovog zadatka.</span><span class="sxs-lookup"><span data-stu-id="ae36d-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="ae36d-113">Evo primjera izmjene globalne politike sastanka za vašu organizaciju.</span><span class="sxs-lookup"><span data-stu-id="ae36d-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="ae36d-114">(Obavezno pregledajte prethodno navedenu dokumentaciju prije nego što učinite te promjene da biste razumjeli što to omogućuje.)</span><span class="sxs-lookup"><span data-stu-id="ae36d-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="ae36d-115">Set-Csteamsmetingpolicy-identitet globalni-AutoAdmittedUsers "svi"-dozvoljena Pstnuserstobypasslobby $True</span><span class="sxs-lookup"><span data-stu-id="ae36d-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="ae36d-116">Za više informacija pogledajte [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="ae36d-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
