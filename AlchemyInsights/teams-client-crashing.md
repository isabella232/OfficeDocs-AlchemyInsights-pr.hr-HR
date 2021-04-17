---
title: Klijent za Teams se ruši?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826263"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="610fa-102">Klijent za Teams se ruši?</span><span class="sxs-lookup"><span data-stu-id="610fa-102">Teams client crashing?</span></span>

<span data-ttu-id="610fa-103">Ako vam se klijent za Teams ruši, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="610fa-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="610fa-104">Ako koristite Teams za stolna računala, [provjerite je li program u potpunosti ažuriran](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="610fa-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="610fa-105">Provjerite jesu li dostupni svi URL-ovi i rasponi adresa za [Microsoft 365.](https://docs.microsoft.com/microsoftteams/connectivity-issues)</span><span class="sxs-lookup"><span data-stu-id="610fa-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="610fa-106">Prijavite se pomoću administratorskog računa klijenta i provjerite nadzornu ploču [stanja](https://docs.microsoft.com/office365/enterprise/view-service-health) servisa da biste provjerili ne postoji li nedostatak ili degradacija servisa.</span><span class="sxs-lookup"><span data-stu-id="610fa-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="610fa-107">Deinstalacija i ponovna instalacija aplikacije Teams (veza)</span><span class="sxs-lookup"><span data-stu-id="610fa-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="610fa-108">Pronađite mapu %appdata%\Microsoft\teams\ na računalu i izbrišite sve datoteke u tom direktoriju.</span><span class="sxs-lookup"><span data-stu-id="610fa-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="610fa-109">[Preuzmite i instalirajte aplikaciju Teams,](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)a ako je moguće, instalirajte Teams kao administrator (desnom tipkom miša kliknite instalacijski program aplikacije Teams i odaberite "Pokreni kao administrator" ako je dostupno).</span><span class="sxs-lookup"><span data-stu-id="610fa-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="610fa-110">Ako se klijent za Teams i dalje ruši, možete li reproducirati problem?</span><span class="sxs-lookup"><span data-stu-id="610fa-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="610fa-111">Ako je tako:</span><span class="sxs-lookup"><span data-stu-id="610fa-111">If so:</span></span>

1. <span data-ttu-id="610fa-112">Pomoću snimača koraka snimite korake.</span><span class="sxs-lookup"><span data-stu-id="610fa-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="610fa-113">Zatvorite sve nepotrebne ili povjerljive aplikacije.</span><span class="sxs-lookup"><span data-stu-id="610fa-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="610fa-114">Pokrenite snimač koraka i reproducirajte problem dok ste prijavljeni s zahvaćenim korisničkim računom.</span><span class="sxs-lookup"><span data-stu-id="610fa-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="610fa-115">[Prikupite zapisnike timova koji snimaju snimljene korake za reprodukciju](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="610fa-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="610fa-116">**Napomena**: provjerite jeste li snimili adresu za prijavu na koju je korisnik na to utječe.</span><span class="sxs-lookup"><span data-stu-id="610fa-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="610fa-117">Prikupite podatke o smetlišu i/ili košu kvara (Windows).</span><span class="sxs-lookup"><span data-stu-id="610fa-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="610fa-118">Pokrenite Windows Powershell na računalu na kojem se ruši i pokrenite sljedeće naredbe:</span><span class="sxs-lookup"><span data-stu-id="610fa-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="610fa-119">Priložite datoteku na slučaj podrške.</span><span class="sxs-lookup"><span data-stu-id="610fa-119">Attach the file to your support case.</span></span>
