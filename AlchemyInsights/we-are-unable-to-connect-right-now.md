---
title: Problem s aktivacijom – trenutno se ne možemo povezati
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725975"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="e56b6-102">Rješavanje aplikacija Microsoft 365 "trenutno se ne možemo povezati" s porukom</span><span class="sxs-lookup"><span data-stu-id="e56b6-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="e56b6-103">Ako primite ovu poruku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="e56b6-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e56b6-104">Provjerite vatrozid, antivirusni softver i postavke proxy poslužitelja da biste potvrdili da ne blokiraju pristup internetu u aplikacije Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e56b6-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="e56b6-105">Pročitajte članak [Microsoftovi URL-ovi i rasponi IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e56b6-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="e56b6-106">Idite na **početak**  >  **pokretanja**, a zatim upišite **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="e56b6-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="e56b6-107">Provjerite jesu li svi sljedeći servisi pokrenuti:</span><span class="sxs-lookup"><span data-stu-id="e56b6-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="e56b6-108">Automatsko postavljanje mrežnih povezanih uređaja</span><span class="sxs-lookup"><span data-stu-id="e56b6-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="e56b6-109">Servis mrežnog popisa</span><span class="sxs-lookup"><span data-stu-id="e56b6-109">Network List Service</span></span>
    - <span data-ttu-id="e56b6-110">Svijest o mrežnom mjestu</span><span class="sxs-lookup"><span data-stu-id="e56b6-110">Network Location Awareness</span></span>
    - <span data-ttu-id="e56b6-111">Zapisnik događaja u sustavu Windows</span><span class="sxs-lookup"><span data-stu-id="e56b6-111">Windows Event Log</span></span>

<span data-ttu-id="e56b6-112">Ako jedan od tih servisa nije pokrenut, pokušajte ga pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="e56b6-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="e56b6-113">Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu otvaranjem naredbenog upita s dodatnim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="e56b6-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="e56b6-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="e56b6-114">**sfc /scannow**</span></span>

<span data-ttu-id="e56b6-115">Kada naredba završi, ponovno pokrenite računalo.</span><span class="sxs-lookup"><span data-stu-id="e56b6-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="e56b6-116">Detaljne informacije potražite u članku ["Žao nam je, ne možemo se povezati s vašim računom. Pokušajte ponovno kasnije "pogreška prilikom aktivacije sustava Office iz programa Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="e56b6-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>