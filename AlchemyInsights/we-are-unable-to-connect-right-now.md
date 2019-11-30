---
title: Problem s aktivacijom-trenutno se ne možemo povezati
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628234"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="59ca3-102">Popravljanje aplikacija sustava Office "ne možemo se odmah povezati" poruka</span><span class="sxs-lookup"><span data-stu-id="59ca3-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="59ca3-103">Ako primite ovu poruku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="59ca3-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="59ca3-104">Provjerite vatrozid, antivirusni softver i postavke proxyja da biste potvrdili da ne blokiraju pristup internetu aplikacijama sustava Office.</span><span class="sxs-lookup"><span data-stu-id="59ca3-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="59ca3-105">Pogledajte [Office 365 URL-ove i IP adrese raspona](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="59ca3-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="59ca3-106">Idite na **pokretanje** > **, a**zatim upišite **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="59ca3-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="59ca3-107">Provjerite jesu li sve sljedeće usluge pokrenite:</span><span class="sxs-lookup"><span data-stu-id="59ca3-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="59ca3-108">Automatsko podešavanje uređaja povezanih s mrežom</span><span class="sxs-lookup"><span data-stu-id="59ca3-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="59ca3-109">Servis popisa mrežnih usluga</span><span class="sxs-lookup"><span data-stu-id="59ca3-109">Network List Service</span></span>
    - <span data-ttu-id="59ca3-110">Svijest o mrežnom mjestu</span><span class="sxs-lookup"><span data-stu-id="59ca3-110">Network Location Awareness</span></span>
    - <span data-ttu-id="59ca3-111">Zapisnik događaja u sustavu Windows</span><span class="sxs-lookup"><span data-stu-id="59ca3-111">Windows Event Log</span></span>

<span data-ttu-id="59ca3-112">Ako jedna od tih usluga nije pokrenut, pokušajte ga pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="59ca3-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="59ca3-113">Ako imate problem s započinjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog retka s povišenim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="59ca3-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="59ca3-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="59ca3-114">**sfc /scannow**</span></span>

<span data-ttu-id="59ca3-115">Nakon završetka ove naredbe, ponovo pokrenite računalo.</span><span class="sxs-lookup"><span data-stu-id="59ca3-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="59ca3-116">Detaljne informacije potražite u stranici ["Žao mi je, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije "pogreška kada aktivirate Office iz Officea 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="59ca3-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>