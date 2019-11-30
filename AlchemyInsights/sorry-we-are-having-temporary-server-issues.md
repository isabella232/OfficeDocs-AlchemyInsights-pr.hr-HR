---
title: Učvršćivanje Officeovih aplikacija Žao mi je, imamo privremenu poruku o problemima poslužitelja
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627982"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="ae5c6-102">Popravljanje aplikacija sustava Office "Žao mi je, imamo privremene probleme s poslužiteljem"</span><span class="sxs-lookup"><span data-stu-id="ae5c6-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="ae5c6-103">Ako primite ovu poruku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="ae5c6-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ae5c6-104">Provjerite vatrozid, antivirusni softver i postavke proxyja da biste potvrdili da ne blokiraju pristup internetu aplikacijama sustava Office.</span><span class="sxs-lookup"><span data-stu-id="ae5c6-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="ae5c6-105">Pogledajte [Office 365 URL-ove i IP adrese raspona](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="ae5c6-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="ae5c6-106">Idite na **pokretanje** > **, a**zatim upišite **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="ae5c6-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="ae5c6-107">Provjerite jesu li sve sljedeće usluge pokrenite:</span><span class="sxs-lookup"><span data-stu-id="ae5c6-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="ae5c6-108">Automatsko podešavanje uređaja povezanih s mrežom</span><span class="sxs-lookup"><span data-stu-id="ae5c6-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="ae5c6-109">Servis popisa mrežnih usluga</span><span class="sxs-lookup"><span data-stu-id="ae5c6-109">Network List Service</span></span>
    - <span data-ttu-id="ae5c6-110">Svijest o mrežnom mjestu</span><span class="sxs-lookup"><span data-stu-id="ae5c6-110">Network Location Awareness</span></span>
    - <span data-ttu-id="ae5c6-111">Zapisnik događaja u sustavu Windows</span><span class="sxs-lookup"><span data-stu-id="ae5c6-111">Windows Event Log</span></span>

<span data-ttu-id="ae5c6-112">Ako jedna od tih usluga nije pokrenut, pokušajte ga pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="ae5c6-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="ae5c6-113">Ako imate problem s započinjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog retka s povišenim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="ae5c6-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="ae5c6-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="ae5c6-114">**sfc /scannow**</span></span>

<span data-ttu-id="ae5c6-115">Nakon završetka ove naredbe, ponovo pokrenite računalo.</span><span class="sxs-lookup"><span data-stu-id="ae5c6-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="ae5c6-116">Detaljne informacije potražite u stranici ["Žao mi je, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije "pogreška kada aktivirate Office iz Officea 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="ae5c6-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>