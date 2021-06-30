---
title: Teams klijent se ruši
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187713"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="639b0-102">Teams klijent se ruši</span><span class="sxs-lookup"><span data-stu-id="639b0-102">Teams client crashing</span></span>

<span data-ttu-id="639b0-103">Ako vam se klijent za Teams ruši, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="639b0-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="639b0-104">Ako koristite Teams za stolna računala, [provjerite je li program u potpunosti ažuriran](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="639b0-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="639b0-105">Provjerite jesu li [dostupni Microsoft 365 URL-ovi](/microsoftteams/connectivity-issues) i rasponi adresa.</span><span class="sxs-lookup"><span data-stu-id="639b0-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="639b0-106">Prijavite se pomoću administratorskog računa klijenta i provjerite nadzornu ploču [stanja](/office365/enterprise/view-service-health) servisa da biste provjerili ne postoji li nedostatak ili degradacija servisa.</span><span class="sxs-lookup"><span data-stu-id="639b0-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="639b0-107">Deinstalacija i ponovna instalacija Teams aplikacije</span><span class="sxs-lookup"><span data-stu-id="639b0-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="639b0-108">Pronađite mapu %appdata%\Microsoft\Teams\ na računalu i izbrišite sve datoteke u tom direktoriju.</span><span class="sxs-lookup"><span data-stu-id="639b0-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="639b0-109">[Preuzmite i instalirajte aplikaciju Teams ,](https://www.microsoft.com/microsoft-teams/download-app)a ako je moguće, instalirajte Teams kao administrator (desnom tipkom miša kliknite instalacijski program Teams pa odaberite **Pokreni kao administrator** ako je dostupan).</span><span class="sxs-lookup"><span data-stu-id="639b0-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="639b0-110">Ako se Teams i dalje ruši, pokušajte reproducirati problem.</span><span class="sxs-lookup"><span data-stu-id="639b0-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="639b0-111">Ako možete:</span><span class="sxs-lookup"><span data-stu-id="639b0-111">If you can:</span></span>

1. <span data-ttu-id="639b0-112">Pomoću snimača koraka snimite korake.</span><span class="sxs-lookup"><span data-stu-id="639b0-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="639b0-113">Zatvorite sve nepotrebne ili povjerljive aplikacije.</span><span class="sxs-lookup"><span data-stu-id="639b0-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="639b0-114">Pokrenite snimač koraka i reproducirajte problem dok ste prijavljeni s zahvaćenim korisničkim računom.</span><span class="sxs-lookup"><span data-stu-id="639b0-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="639b0-115">[Prikupite zapisnike timova koji snimaju snimljene korake za reprodukciju](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="639b0-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="639b0-116">**Napomena**: provjerite jeste li snimili adresu za prijavu na koju je korisnik na to utječe.</span><span class="sxs-lookup"><span data-stu-id="639b0-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="639b0-117">Prikupite podatke o izvatkom i/ili košu kvara (Windows).</span><span class="sxs-lookup"><span data-stu-id="639b0-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="639b0-118">Pokrenite Windows powershell na uređaju na kojem se ruši i pokrenite sljedeće naredbe (nakon svake naredbe pritisnite Enter):</span><span class="sxs-lookup"><span data-stu-id="639b0-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="639b0-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="639b0-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="639b0-120">Kada se tekstna datoteka generira i prikaže na zaslonu, spremite datoteku i priložite je zahtjevu za servis.</span><span class="sxs-lookup"><span data-stu-id="639b0-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
