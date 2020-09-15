---
title: Hodnik za zaobilaženje
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684942"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="1a45d-102">Upravljanje postavkama predvorja i razinom sudjelovanja u timovima</span><span class="sxs-lookup"><span data-stu-id="1a45d-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="1a45d-103">Ako želite dopustiti svima, uključujući biranjem, vanjskim i anonimnim korisnicima, **zaobići predvorje**, pomoću komponente PowerShell možete izvršiti ovaj zadatak.</span><span class="sxs-lookup"><span data-stu-id="1a45d-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="1a45d-104">Evo primjera izmjene pravilnika globalnog sastanka za vašu tvrtku ili ustanovu.</span><span class="sxs-lookup"><span data-stu-id="1a45d-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="1a45d-105">Ovaj cmdlet trenutno zahtijeva korištenje modula za Skype za tvrtke PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1a45d-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="1a45d-106">Da biste se postavili za korištenje tog cmdleta, pogledajte [Upravljanje pravilima pomoću komponente PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="1a45d-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="1a45d-107">Kada postavite pravilnik, morate ga primijeniti na korisnike; Ako ste izmijenili globalno pravilo, ona će se automatski primijeniti na korisnike.</span><span class="sxs-lookup"><span data-stu-id="1a45d-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="1a45d-108">Za bilo koju promjenu pravila morate čekati najmanje **4 sata do 24 sata** da bi pravila stupila na utjecaj.</span><span class="sxs-lookup"><span data-stu-id="1a45d-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="1a45d-109">Obavezno pregledajte dokumentaciju u nastavku prije nego što ove promjene razumijete točno što to omogućuje.</span><span class="sxs-lookup"><span data-stu-id="1a45d-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="1a45d-110">Upravljanje pravilima predvorja za sastanke s timovima</span><span class="sxs-lookup"><span data-stu-id="1a45d-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="1a45d-111">Te postavke kontroliraju sudionike sastanka koji čekaju u predvorju prije nego što ih prime na sastanak i na razinu sudjelovanja koje im je dopušteno na sastanku.</span><span class="sxs-lookup"><span data-stu-id="1a45d-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="1a45d-112">Pomoću komponente PowerShell možete ažurirati postavke pravilnika sastanka koje još nisu implementirane (s oznakom "uskoro") u centru za administratore timova.</span><span class="sxs-lookup"><span data-stu-id="1a45d-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="1a45d-113">U nastavku potražite ogledni cmdlet za PowerShell koji korisnicima omogućuje zaobilaženje predvorja.</span><span class="sxs-lookup"><span data-stu-id="1a45d-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="1a45d-114">[Automatski Priznajte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) da su korisnici po pravilima organizatora koji kontroliraju hoće li se osobe izravno pridružiti sastanku ili čekati u predvorju dok ih ne prizna ovjereni korisnik.</span><span class="sxs-lookup"><span data-stu-id="1a45d-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="1a45d-115">[Dopuštanje anonimnih osoba da pokrene sastanak](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) jest pravilo po organizatoru koje kontrolira jesu li anonimni osobe, uključujući B2B i udruženu korisnike, mogli sudjelovati u sastanku korisnika bez ovlaštenog korisnika iz tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="1a45d-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="1a45d-116">[Dopusti korisnicima biranjem zaobilaženje predvorja](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**uskoro**) je pravilo po organizatoru koje kontrolira hoće li se osobe koje se biraju putem telefona izravno pridružiti sastanku ili čekati u predvorju bez obzira na to da **automatski priznaju postavljanje osoba** .</span><span class="sxs-lookup"><span data-stu-id="1a45d-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="1a45d-117">[Dopusti organizatorima da nadjačaju postavke predvorja](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**uskoro**) predstavlja pravilnik o organizatoru koja kontrolira može li organizator sastanka nadjačati postavke predvorja koje je administrator postavio **automatski priznaje osobe** i **Dopusti korisnicima biranjem zaobilaženje predvorja** prilikom zakazivanja novog sastanka.</span><span class="sxs-lookup"><span data-stu-id="1a45d-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="1a45d-118">**Upozorenje:** Pročitajte [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) za potpuni pregled pravilnika o sastanku u Microsoftovim timovima.</span><span class="sxs-lookup"><span data-stu-id="1a45d-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
