---
title: Klijent za Teams se ruši?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691099"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="aeca2-102">Klijent za Teams se ruši?</span><span class="sxs-lookup"><span data-stu-id="aeca2-102">Teams client crashing?</span></span>

<span data-ttu-id="aeca2-103">Ako vam se klijent za Teams ruši, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="aeca2-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="aeca2-104">Ako koristite Teams za stolna računala, [provjerite je li program u potpunosti ažuriran](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="aeca2-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="aeca2-105">Provjerite jesu li svi [URL-ovi i rasponi microsoftova 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) dostupni.</span><span class="sxs-lookup"><span data-stu-id="aeca2-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="aeca2-106">Prijavite se pomoću računa za administratore korisnika i provjerite postoji li [kontrolna tabla zdravstvenog stanja](https://docs.microsoft.com/office365/enterprise/view-service-health) da biste provjerili postoji li propadanje ili degradacija servisa.</span><span class="sxs-lookup"><span data-stu-id="aeca2-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="aeca2-107">Deinstalacija i ponovna instalacija aplikacije timovi (veza)</span><span class="sxs-lookup"><span data-stu-id="aeca2-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="aeca2-108">Dođite do% AppData%\microsoft\teams\ folder na računalu i izbrišite sve datoteke u tom direktoriju.</span><span class="sxs-lookup"><span data-stu-id="aeca2-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="aeca2-109">[Preuzmite i instalirajte aplikaciju timovi](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), a ako je moguće, instalirajte timove kao administratore (desnom tipkom miša kliknite instalacijski program za timove, a zatim odaberite "Pokreni kao administrator" Ako je dostupno).</span><span class="sxs-lookup"><span data-stu-id="aeca2-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="aeca2-110">Ako vam se klijent za timove i dalje ruši, možete li ponoviti problem?</span><span class="sxs-lookup"><span data-stu-id="aeca2-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="aeca2-111">Ako je tako, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="aeca2-111">If so:</span></span>

1. <span data-ttu-id="aeca2-112">Upotrijebite snimač koraka da biste snimili korake.</span><span class="sxs-lookup"><span data-stu-id="aeca2-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="aeca2-113">Zatvaranje svih nepotrebnih ili povjerljivih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="aeca2-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="aeca2-114">Pokrenite snimač koraka i reproducirajte problem dok ste prijavljeni uz izvještačen korisnički račun.</span><span class="sxs-lookup"><span data-stu-id="aeca2-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="aeca2-115">[Prikupite zapisnike timova koji snimaju snimljene reproducirajte korake](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="aeca2-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="aeca2-116">**Pažnja**: Provjerite jeste li snimili adresu za prijavu na korisnika koji je utjecao na njega.</span><span class="sxs-lookup"><span data-stu-id="aeca2-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="aeca2-117">Prikupljanje podataka o izvatkom i/ili kvaru (Windows).</span><span class="sxs-lookup"><span data-stu-id="aeca2-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="aeca2-118">Pokrenite Windows PowerShell na stroju na kojem se pojavljuje sudar i pokrenite sljedeće naredbe:</span><span class="sxs-lookup"><span data-stu-id="aeca2-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="aeca2-119">Priložite datoteku u slučaj podrške.</span><span class="sxs-lookup"><span data-stu-id="aeca2-119">Attach the file to your support case.</span></span>
