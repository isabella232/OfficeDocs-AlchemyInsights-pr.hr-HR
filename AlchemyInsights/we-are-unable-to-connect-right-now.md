---
title: Aktivacija Issue - Nismo u mogućnosti to povezivanje odmah
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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581867"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="83408-102">Popravljanje poruke aplikacije Microsoft 365 "Trenutno se ne možemo povezati"</span><span class="sxs-lookup"><span data-stu-id="83408-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="83408-103">Ako primite ovu poruku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="83408-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="83408-104">Provjerite postavke vatrozida, antivirusnog softvera i proxy poslužitelja da biste potvrdili da ne blokiraju pristup internetu aplikacijama sustava Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="83408-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="83408-105">Pogledajte [Microsoftove URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="83408-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="83408-106">Idite na **Pokreni**  >  **,** a zatim upišite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="83408-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="83408-107">Provjerite jesu li pokrenuti sljedeći servisi:</span><span class="sxs-lookup"><span data-stu-id="83408-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="83408-108">Automatsko postavljanje uređaja povezanih s mrežom</span><span class="sxs-lookup"><span data-stu-id="83408-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="83408-109">Usluga mrežnog popisa</span><span class="sxs-lookup"><span data-stu-id="83408-109">Network List Service</span></span>
    - <span data-ttu-id="83408-110">Svijest o mrežnom mjestu</span><span class="sxs-lookup"><span data-stu-id="83408-110">Network Location Awareness</span></span>
    - <span data-ttu-id="83408-111">Zapisnik događaja sustava Windows</span><span class="sxs-lookup"><span data-stu-id="83408-111">Windows Event Log</span></span>

<span data-ttu-id="83408-112">Ako jedan od tih servisa nije pokrenut, pokušajte ga pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="83408-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="83408-113">Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog retka s povišenim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="83408-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="83408-114">**sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="83408-114">**sfc /scannow**</span></span>

<span data-ttu-id="83408-115">Nakon što ova naredba završi, ponovo pokrenite računalo.</span><span class="sxs-lookup"><span data-stu-id="83408-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="83408-116">Detaljne informacije potražite u [odjeljku "Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije" pogreška kada aktivirate Office iz Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="83408-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>