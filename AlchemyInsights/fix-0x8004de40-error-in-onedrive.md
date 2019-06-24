---
title: Ispravite pogreške 0x8004de40 u OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133969"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="7591b-102">Ispravite pogreške 0x8004de40 u OneDrive</span><span class="sxs-lookup"><span data-stu-id="7591b-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="7591b-103">Ako primite poruku o pogrešci 0x8004de40 s OneDrive:</span><span class="sxs-lookup"><span data-stu-id="7591b-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="7591b-104">Ponovo pokrenite problematično računalo dok ste povezani s aktinvo direktorij domene.</span><span class="sxs-lookup"><span data-stu-id="7591b-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="7591b-105">Ako ponovno pokretanje ne riješi problem, odvajanja od i ponovno se pridružite uređaj iz Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7591b-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="7591b-106">**Napomena**: treba biti na mreži tvrtke prilikom izvođenja ove korake.</span><span class="sxs-lookup"><span data-stu-id="7591b-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="7591b-107">Ne izvršite ove kada niste moći povezati s korporacijskom Infrastruktura (na primjer, tijekom putovanja).</span><span class="sxs-lookup"><span data-stu-id="7591b-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="7591b-108">Otvorite privilegiranom naredbenom retku.</span><span class="sxs-lookup"><span data-stu-id="7591b-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="7591b-109">Da biste otvorili privilegirani naredbeni redak, kliknite - **Start**, desnom tipkom miša kliknite **naredbeni redak**i zatim kliknite **Pokreni kao administrator**.</span><span class="sxs-lookup"><span data-stu-id="7591b-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="7591b-110">Upišite *dsregcmd /leave* i pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="7591b-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="7591b-111">Kada je dovršeno, upišite *dsregcmd /join* i pritisnite tipku **Enter**.</span><span class="sxs-lookup"><span data-stu-id="7591b-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="7591b-112">Kad je dovršeno, zatvorite naredbeni redak.</span><span class="sxs-lookup"><span data-stu-id="7591b-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="7591b-113">Ponovno pokrenite računalo i prijavite se u OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7591b-113">Reboot the computer, and log into OneDrive.</span></span>