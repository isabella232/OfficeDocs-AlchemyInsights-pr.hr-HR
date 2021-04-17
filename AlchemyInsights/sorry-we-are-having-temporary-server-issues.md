---
title: Rješavanje problema s aplikacijom Microsoft 365 Nažalost, imamo poruku o privremenim problemima s poslužiteljem
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835263"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="3bc47-102">Popravljanje aplikacije Microsoft 365 "Nažalost, imamo privremene probleme s poslužiteljem"</span><span class="sxs-lookup"><span data-stu-id="3bc47-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="3bc47-103">Ako primite ovu poruku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="3bc47-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="3bc47-104">Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste potvrdili da ne blokiraju pristup internetu aplikacijama Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3bc47-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="3bc47-105">Pogledajte [URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="3bc47-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="3bc47-106">Idite na **Pokreni**  >  **pokreni**, a zatim upišite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="3bc47-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="3bc47-107">Provjerite jesu li svi sljedeći servisi pokrenuti:</span><span class="sxs-lookup"><span data-stu-id="3bc47-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="3bc47-108">Automatsko postavljanje mrežnih uređaja</span><span class="sxs-lookup"><span data-stu-id="3bc47-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="3bc47-109">Servis za mrežni popis</span><span class="sxs-lookup"><span data-stu-id="3bc47-109">Network List Service</span></span>
    - <span data-ttu-id="3bc47-110">Svijesti o mrežnom mjestu</span><span class="sxs-lookup"><span data-stu-id="3bc47-110">Network Location Awareness</span></span>
    - <span data-ttu-id="3bc47-111">Zapisnik događaja u sustavu Windows</span><span class="sxs-lookup"><span data-stu-id="3bc47-111">Windows Event Log</span></span>

<span data-ttu-id="3bc47-112">Ako neki od tih servisa nije pokrenut, pokušajte ga pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="3bc47-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="3bc47-113">Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu tako da otvorite naredbeni redak s dodatnim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="3bc47-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="3bc47-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="3bc47-114">**sfc /scannow**</span></span>

<span data-ttu-id="3bc47-115">Kada ova naredba završi, ponovno pokrenite računalo.</span><span class="sxs-lookup"><span data-stu-id="3bc47-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="3bc47-116">Detaljne informacije potražite u članku ["Nažalost, ne možemo se povezati s vašim računom. Kada aktivirate, pokušajte ponovno kasnije".](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="3bc47-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>