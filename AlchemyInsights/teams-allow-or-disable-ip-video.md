---
title: Timovi omogućuju ili onemogućuju IP videozapis
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670176"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="de868-102">Timovi omogućuju ili onemogućuju IP videozapis</span><span class="sxs-lookup"><span data-stu-id="de868-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="de868-103">**Promjena ili stvaranje pravilnika sastanka**</span><span class="sxs-lookup"><span data-stu-id="de868-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="de868-104">Da biste promijenili ili stvorili pravilnik o sastanku, otvorite **centar za administratore programa Microsoft timovi > sastanci > pravilima sastanka**.</span><span class="sxs-lookup"><span data-stu-id="de868-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="de868-105">Odaberite pravilnik s popisa ili kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="de868-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="de868-106">Ako stvarate novi pravilnik, dodajte mu naziv i opis.</span><span class="sxs-lookup"><span data-stu-id="de868-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="de868-107">Naziv ne može sadržavati posebne znakove ni biti dulji od 64 znaka.</span><span class="sxs-lookup"><span data-stu-id="de868-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="de868-108">Odaberite postavke, a zatim kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="de868-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="de868-109">Primjerice, recimo da imate mnogo korisnika i želite ograničiti količinu propusnosti koju bi njihov sastanak zahtijevao.</span><span class="sxs-lookup"><span data-stu-id="de868-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="de868-110">Stvorili biste novi prilagođeni pravilnik pod nazivom „Ograničena propusnost” i onemogućili ove postavke:</span><span class="sxs-lookup"><span data-stu-id="de868-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="de868-111">U odjeljku **Audio i video**:</span><span class="sxs-lookup"><span data-stu-id="de868-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="de868-112">Isključite Dopusti snimanje u oblaku.</span><span class="sxs-lookup"><span data-stu-id="de868-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="de868-113">Isključite Dopusti IP videozapise.</span><span class="sxs-lookup"><span data-stu-id="de868-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="de868-114">Potom dodijelite pravilnik korisnicima.</span><span class="sxs-lookup"><span data-stu-id="de868-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="de868-115">**Dodjeljivanje pravilnika za sastanke korisnicima**</span><span class="sxs-lookup"><span data-stu-id="de868-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="de868-116">U lijevom navigacijskom oknu centra za administratore programa Microsoft Teams idite na odjeljak **Korisnici**, a zatim kliknite korisnika.</span><span class="sxs-lookup"><span data-stu-id="de868-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="de868-117">Odaberite korisnika tako da kliknete lijevo od njegovog imena, a zatim kliknete **Uređivanje postavki**.</span><span class="sxs-lookup"><span data-stu-id="de868-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="de868-118">U odjeljku **pravilnik o sastanku**odaberite pravilo koje želite dodijeliti, a zatim kliknite **Primijeni**.</span><span class="sxs-lookup"><span data-stu-id="de868-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="de868-119">Dodatne informacije potražite u članku [Upravljanje pravilima sastanka u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="de868-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
