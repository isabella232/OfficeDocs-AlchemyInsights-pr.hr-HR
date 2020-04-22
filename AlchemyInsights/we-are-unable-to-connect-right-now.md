---
title: Problem s aktivacijom – trenutno se ne možemo povezati
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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716164"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="826af-102">Popravljanje poruke aplikacije sustava Office "Trenutno se ne možemo povezati"</span><span class="sxs-lookup"><span data-stu-id="826af-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="826af-103">Ako primite ovu poruku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="826af-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="826af-104">Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste potvrdili da ne blokiraju pristup internetu aplikacijama sustava Office.</span><span class="sxs-lookup"><span data-stu-id="826af-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="826af-105">Pogledajte [Microsoftove URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="826af-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="826af-106">Idite na **Pokreni** > **,** a zatim upišite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="826af-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="826af-107">Provjerite jesu li pokrenuti sljedeći servisi:</span><span class="sxs-lookup"><span data-stu-id="826af-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="826af-108">Automatsko postavljanje mrežnih povezanih uređaja</span><span class="sxs-lookup"><span data-stu-id="826af-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="826af-109">Usluga popisa mreža</span><span class="sxs-lookup"><span data-stu-id="826af-109">Network List Service</span></span>
    - <span data-ttu-id="826af-110">Svijest o mrežnom mjestu</span><span class="sxs-lookup"><span data-stu-id="826af-110">Network Location Awareness</span></span>
    - <span data-ttu-id="826af-111">Zapisnik događaja u sustavu Windows</span><span class="sxs-lookup"><span data-stu-id="826af-111">Windows Event Log</span></span>

<span data-ttu-id="826af-112">Ako se jedna od tih usluga ne izvodi, pokušajte ga pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="826af-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="826af-113">Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog retka s povišenim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="826af-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="826af-114">**sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="826af-114">**sfc /scannow**</span></span>

<span data-ttu-id="826af-115">Nakon dovršetka ove naredbe ponovo pokrenite računalo.</span><span class="sxs-lookup"><span data-stu-id="826af-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="826af-116">Detaljne informacije potražite u [odjeljku "Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovo kasnije" kada aktivirate Office iz sustava Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="826af-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>