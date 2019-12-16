---
title: Fix 0x8004de40 pogreška u servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052029"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="ea5fe-102">Fix 0x8004de40 pogreška u servisu OneDrive</span><span class="sxs-lookup"><span data-stu-id="ea5fe-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="ea5fe-103">Ako primite pogrešku 0x8004de40 s servisom OneDrive:</span><span class="sxs-lookup"><span data-stu-id="ea5fe-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="ea5fe-104">Ponovno pokrenite zahvaćeno računalo dok ste spojeni na svoju domenu Acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="ea5fe-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="ea5fe-105">Ako ponovno pokretanje ne popravi problem, nepridružite se i ponovno pridružite uređaju iz servisa Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ea5fe-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="ea5fe-106">**Napomena**: trebali biste biti na korporacijskoj mreži tijekom izvođenja ovih koraka.</span><span class="sxs-lookup"><span data-stu-id="ea5fe-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="ea5fe-107">Nemojte obavljati ove korake kada se ne možete povezati s korporativnom infrastrukturom (na primjer, tijekom putovanja).</span><span class="sxs-lookup"><span data-stu-id="ea5fe-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="ea5fe-108">Otvorite povećani naredbeni redak.</span><span class="sxs-lookup"><span data-stu-id="ea5fe-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="ea5fe-109">Da biste otvorili povećani naredbeni redak, kliknite- **Start**, desnom tipkom miša kliknite **naredbeni redak**, a zatim kliknite **Pokreni kao administrator**.</span><span class="sxs-lookup"><span data-stu-id="ea5fe-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="ea5fe-110">Upišite *dsregcmd/dopust* i pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="ea5fe-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="ea5fe-111">Kada dovršite, upišite *dsregcmd/Join* i pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="ea5fe-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="ea5fe-112">Kada završite, zatvorite naredbeni redak.</span><span class="sxs-lookup"><span data-stu-id="ea5fe-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="ea5fe-113">Ponovno pokrenite računalo i prijavite se na OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ea5fe-113">Reboot the computer, and log into OneDrive.</span></span>