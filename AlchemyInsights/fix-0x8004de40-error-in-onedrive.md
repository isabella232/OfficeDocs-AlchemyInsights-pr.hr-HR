---
title: Ispravite pogreške 0x8004de40 u OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755840"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="9c599-102">Ispravite pogreške 0x8004de40 u OneDrive</span><span class="sxs-lookup"><span data-stu-id="9c599-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="9c599-103">Ako primite poruku o pogrešci 0x8004de40 s OneDrive:</span><span class="sxs-lookup"><span data-stu-id="9c599-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="9c599-104">Ponovo pokrenite problematično računalo dok ste povezani s aktinvo direktorij domene.</span><span class="sxs-lookup"><span data-stu-id="9c599-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="9c599-105">Ako ponovno pokretanje ne riješi problem, odvajanja od i ponovno se pridružite uređaj iz Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9c599-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="9c599-106">**Napomena**: treba biti na mreži tvrtke prilikom izvođenja ove korake.</span><span class="sxs-lookup"><span data-stu-id="9c599-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="9c599-107">Ne izvršite ove kada niste moći povezati s korporacijskom Infrastruktura (na primjer, tijekom putovanja).</span><span class="sxs-lookup"><span data-stu-id="9c599-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="9c599-108">Otvorite privilegiranom naredbenom retku.</span><span class="sxs-lookup"><span data-stu-id="9c599-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="9c599-109">Da biste otvorili privilegirani naredbeni redak, kliknite - **Start**, desnom tipkom miša kliknite **naredbeni redak**i zatim kliknite **Pokreni kao administrator**.</span><span class="sxs-lookup"><span data-stu-id="9c599-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="9c599-110">Upišite *dsregcmd /leave* i pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="9c599-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="9c599-111">Kada je dovršeno, upišite *dsregcmd /join* i pritisnite tipku **Enter**.</span><span class="sxs-lookup"><span data-stu-id="9c599-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="9c599-112">Kad je dovršeno, zatvorite naredbeni redak.</span><span class="sxs-lookup"><span data-stu-id="9c599-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="9c599-113">Ponovno pokrenite računalo i prijavite se u OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9c599-113">Reboot the computer, and log into OneDrive.</span></span>