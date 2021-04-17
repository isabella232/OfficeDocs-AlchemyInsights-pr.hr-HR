---
title: Teams dopušta ili onemogućuje IP videozapis
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826335"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="6b56d-102">Teams dopušta ili onemogućuje IP videozapis</span><span class="sxs-lookup"><span data-stu-id="6b56d-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="6b56d-103">**Promjena ili stvaranje pravilnika sastanka**</span><span class="sxs-lookup"><span data-stu-id="6b56d-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="6b56d-104">Da biste promijenili ili stvorili pravilnik za sastanke, idite u centar za administratore aplikacije **Microsoft Teams > sastancima > sastanaka**.</span><span class="sxs-lookup"><span data-stu-id="6b56d-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="6b56d-105">Odaberite pravilnik s popisa ili kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="6b56d-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="6b56d-106">Ako stvarate novi pravilnik, dodajte mu naziv i opis.</span><span class="sxs-lookup"><span data-stu-id="6b56d-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="6b56d-107">Naziv ne može sadržavati posebne znakove ni biti dulji od 64 znaka.</span><span class="sxs-lookup"><span data-stu-id="6b56d-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="6b56d-108">Odaberite postavke, a zatim kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="6b56d-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="6b56d-109">Recimo, primjerice, da imate mnogo korisnika i želite ograničiti količinu propusnosti koju bi sastanak trebao.</span><span class="sxs-lookup"><span data-stu-id="6b56d-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="6b56d-110">Stvorili biste novi prilagođeni pravilnik pod nazivom „Ograničena propusnost” i onemogućili ove postavke:</span><span class="sxs-lookup"><span data-stu-id="6b56d-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="6b56d-111">U odjeljku **Audio i video**:</span><span class="sxs-lookup"><span data-stu-id="6b56d-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="6b56d-112">Isključite Dopusti snimanje u oblaku.</span><span class="sxs-lookup"><span data-stu-id="6b56d-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="6b56d-113">Isključite Dopusti IP videozapise.</span><span class="sxs-lookup"><span data-stu-id="6b56d-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="6b56d-114">Potom dodijelite pravilnik korisnicima.</span><span class="sxs-lookup"><span data-stu-id="6b56d-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="6b56d-115">**Dodjeljivanje pravilnika za sastanke korisnicima**</span><span class="sxs-lookup"><span data-stu-id="6b56d-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="6b56d-116">U lijevom navigacijskom oknu centra za administratore programa Microsoft Teams idite na odjeljak **Korisnici**, a zatim kliknite korisnika.</span><span class="sxs-lookup"><span data-stu-id="6b56d-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="6b56d-117">Odaberite korisnika tako da kliknete lijevo od njegovog imena, a zatim kliknete **Uređivanje postavki**.</span><span class="sxs-lookup"><span data-stu-id="6b56d-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="6b56d-118">U **odjeljku Pravilnik** o sastanku odaberite pravilnik koji želite dodijeliti, a zatim **kliknite Primijeni**.</span><span class="sxs-lookup"><span data-stu-id="6b56d-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="6b56d-119">Dodatne informacije potražite u članku Upravljanje pravilima [sastanka u aplikaciji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="6b56d-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
