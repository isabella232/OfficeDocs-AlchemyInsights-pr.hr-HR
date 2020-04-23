---
title: Popravak pogreške 0x8004de40 na servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716020"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="4e8f7-102">Popravak pogreške 0x8004de40 na servisu OneDrive</span><span class="sxs-lookup"><span data-stu-id="4e8f7-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="4e8f7-103">Ako primite poruku o pogrešci 0x8004de40 sa servisom OneDrive:</span><span class="sxs-lookup"><span data-stu-id="4e8f7-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="4e8f7-104">Ponovno podizanje sustava izvještačen računalo kratak vremenski razmak povezivanje to tvoj Acitve Imenik domena.</span><span class="sxs-lookup"><span data-stu-id="4e8f7-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="4e8f7-105">Ako ponovno pokretanje ne riješi problem, poništite vezu i ponovno se pridružite uređaju iz azure AD-a.</span><span class="sxs-lookup"><span data-stu-id="4e8f7-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="4e8f7-106">**Napomena:** Trebali biste biti na svojoj korporativnoj mreži tijekom izvođenja ovih koraka.</span><span class="sxs-lookup"><span data-stu-id="4e8f7-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="4e8f7-107">Nemojte izvoditi ove korake kada se ne možete povezati s vašom poslovnom infrastrukturom (na primjer, tijekom putovanja).</span><span class="sxs-lookup"><span data-stu-id="4e8f7-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="4e8f7-108">Otvorite privilegirani naredbeni redak.</span><span class="sxs-lookup"><span data-stu-id="4e8f7-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="4e8f7-109">Da biste otvorili privilegirani naredbeni redak, kliknite – **Start**, desnom tipkom miša kliknite **Naredbeni redak,** a zatim **kliknite Pokreni kao administrator**.</span><span class="sxs-lookup"><span data-stu-id="4e8f7-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="4e8f7-110">Tip *dsregcmd dopust* i prisutan **Ulaziti**.</span><span class="sxs-lookup"><span data-stu-id="4e8f7-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="4e8f7-111">Kada završite, upišite *dsregcmd /join* i pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="4e8f7-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="4e8f7-112">Kada završite, zatvorite naredbeni redak.</span><span class="sxs-lookup"><span data-stu-id="4e8f7-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="4e8f7-113">Ponovno pokrenite računalo i prijavite se na OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4e8f7-113">Reboot the computer, and log into OneDrive.</span></span>