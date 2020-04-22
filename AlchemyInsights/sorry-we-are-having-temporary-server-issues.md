---
title: Popravljanje aplikacija sustava Office Nažalost, imamo poruku o privremenim problemima s poslužiteljem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764109"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="5c8fc-102">Učvršćivanje poruka "Nažalost, imamo privremene probleme s poslužiteljem"</span><span class="sxs-lookup"><span data-stu-id="5c8fc-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="5c8fc-103">Ako primite ovu poruku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="5c8fc-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="5c8fc-104">Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste potvrdili da ne blokiraju pristup internetu aplikacijama sustava Office.</span><span class="sxs-lookup"><span data-stu-id="5c8fc-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="5c8fc-105">Pogledajte [URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="5c8fc-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="5c8fc-106">Idite na **Pokreni** > **,** a zatim upišite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="5c8fc-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="5c8fc-107">Provjerite jesu li pokrenuti sljedeći servisi:</span><span class="sxs-lookup"><span data-stu-id="5c8fc-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="5c8fc-108">Automatsko postavljanje mrežnih povezanih uređaja</span><span class="sxs-lookup"><span data-stu-id="5c8fc-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="5c8fc-109">Usluga popisa mreža</span><span class="sxs-lookup"><span data-stu-id="5c8fc-109">Network List Service</span></span>
    - <span data-ttu-id="5c8fc-110">Svijest o mrežnom mjestu</span><span class="sxs-lookup"><span data-stu-id="5c8fc-110">Network Location Awareness</span></span>
    - <span data-ttu-id="5c8fc-111">Zapisnik događaja u sustavu Windows</span><span class="sxs-lookup"><span data-stu-id="5c8fc-111">Windows Event Log</span></span>

<span data-ttu-id="5c8fc-112">Ako se jedna od tih usluga ne izvodi, pokušajte ga pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="5c8fc-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="5c8fc-113">Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog retka s povišenim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="5c8fc-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="5c8fc-114">**sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="5c8fc-114">**sfc /scannow**</span></span>

<span data-ttu-id="5c8fc-115">Nakon dovršetka ove naredbe ponovo pokrenite računalo.</span><span class="sxs-lookup"><span data-stu-id="5c8fc-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="5c8fc-116">Detaljne informacije potražite u [odjeljku "Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije" pogreška prilikom aktivacije](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="5c8fc-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>