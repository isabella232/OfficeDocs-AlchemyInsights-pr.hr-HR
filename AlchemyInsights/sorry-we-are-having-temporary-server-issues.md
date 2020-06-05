---
title: Popravljanje aplikacija sustava Microsoft 365 Nažalost, imamo poruku o privremenim problemima s poslužiteljem
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582695"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="9855c-102">Ispravak poruke aplikacije Microsoft 365 "Nažalost, imamo privremene probleme s poslužiteljem"</span><span class="sxs-lookup"><span data-stu-id="9855c-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="9855c-103">Ako primite ovu poruku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="9855c-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="9855c-104">Provjerite postavke vatrozida, antivirusnog softvera i proxy poslužitelja da biste potvrdili da ne blokiraju pristup internetu aplikacijama sustava Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9855c-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="9855c-105">Pogledajte [URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="9855c-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="9855c-106">Idite na **Pokreni**  >  **,** a zatim upišite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="9855c-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="9855c-107">Provjerite jesu li pokrenuti sljedeći servisi:</span><span class="sxs-lookup"><span data-stu-id="9855c-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="9855c-108">Automatsko postavljanje uređaja povezanih s mrežom</span><span class="sxs-lookup"><span data-stu-id="9855c-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="9855c-109">Usluga mrežnog popisa</span><span class="sxs-lookup"><span data-stu-id="9855c-109">Network List Service</span></span>
    - <span data-ttu-id="9855c-110">Svijest o mrežnom mjestu</span><span class="sxs-lookup"><span data-stu-id="9855c-110">Network Location Awareness</span></span>
    - <span data-ttu-id="9855c-111">Zapisnik događaja sustava Windows</span><span class="sxs-lookup"><span data-stu-id="9855c-111">Windows Event Log</span></span>

<span data-ttu-id="9855c-112">Ako jedan od tih servisa nije pokrenut, pokušajte ga pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="9855c-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="9855c-113">Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog retka s povišenim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="9855c-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="9855c-114">**sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="9855c-114">**sfc /scannow**</span></span>

<span data-ttu-id="9855c-115">Nakon što ova naredba završi, ponovo pokrenite računalo.</span><span class="sxs-lookup"><span data-stu-id="9855c-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="9855c-116">Detaljne informacije potražite u [odjeljku "Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije" pogreška kada aktivirate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="9855c-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>