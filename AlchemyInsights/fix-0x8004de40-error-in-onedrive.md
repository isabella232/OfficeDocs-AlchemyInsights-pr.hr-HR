---
title: Pogreška za ispravljanje 0x8004de40 na servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745122"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="133a8-102">Pogreška za ispravljanje 0x8004de40 na servisu OneDrive</span><span class="sxs-lookup"><span data-stu-id="133a8-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="133a8-103">Ako vam se prikaže pogreška 0x8004de40 sa servisom OneDrive:</span><span class="sxs-lookup"><span data-stu-id="133a8-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="133a8-104">Ponovno pokrenite računalo koje je utjecalo na nju dok ste povezani s domenom tvrtke Acitve.</span><span class="sxs-lookup"><span data-stu-id="133a8-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="133a8-105">Ako ponovno pokretanje ne riješi problem, poništite pridruživanje i ponovno se pridruži uređaju iz servisa Azure AD.</span><span class="sxs-lookup"><span data-stu-id="133a8-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="133a8-106">**Imajte**na glavi: prilikom izvođenja ovih koraka trebali biste biti na mreži korporativnih tvrtki.</span><span class="sxs-lookup"><span data-stu-id="133a8-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="133a8-107">Ne izvodite ove korake kada se ne možete povezati s korporacijskom infrastrukturom (na primjer, tijekom putovanja).</span><span class="sxs-lookup"><span data-stu-id="133a8-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="133a8-108">Otvaranje povišenog naredbenog upita.</span><span class="sxs-lookup"><span data-stu-id="133a8-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="133a8-109">Da biste otvorili povišeni naredbeni upit, kliknite- **Start**, desnom tipkom miša kliknite **naredbeni upit**, a zatim kliknite **Pokreni kao administrator**.</span><span class="sxs-lookup"><span data-stu-id="133a8-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="133a8-110">Upišite *dsregcmd/ostavite* i pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="133a8-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="133a8-111">Kada završite, upišite *dsregcmd/Join* i pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="133a8-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="133a8-112">Kada završite, zatvaranje naredbenog upita.</span><span class="sxs-lookup"><span data-stu-id="133a8-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="133a8-113">Ponovno pokrenite računalo i prijavite se na OneDrive.</span><span class="sxs-lookup"><span data-stu-id="133a8-113">Reboot the computer, and log into OneDrive.</span></span>