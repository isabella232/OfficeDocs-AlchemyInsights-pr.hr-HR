---
title: Otklanjanje poteškoća sa servisom OneDrive ruši se
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748797"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="84d8b-102">Otklanjanje poteškoća sa servisom OneDrive ruši se</span><span class="sxs-lookup"><span data-stu-id="84d8b-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="84d8b-103">Ako se OneDrive više puta ruši, isprobajte sljedeće korake za otklanjanje poteškoća:</span><span class="sxs-lookup"><span data-stu-id="84d8b-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="84d8b-104">**Provjerite nisu li ključevi registra postavljeni:**</span><span class="sxs-lookup"><span data-stu-id="84d8b-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="84d8b-105">Pomoću uređivača registra idite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="84d8b-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="84d8b-106">Ako je DisableFileSyncNGSC prisutan i postavljen na 1, otvorite tipku i promijenite vrijednost na 0.</span><span class="sxs-lookup"><span data-stu-id="84d8b-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="84d8b-107">Ručno pokretanje servisa OneDrive tako da otvorite Start</span><span class="sxs-lookup"><span data-stu-id="84d8b-107">Manually launch OneDrive by going to Start</span></span> ![Pritisnite tipku Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="84d8b-109">, u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.</span><span class="sxs-lookup"><span data-stu-id="84d8b-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="84d8b-110">**Vraćanje izvornih postavki servisa OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="84d8b-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="84d8b-111">Bilješke:</span><span class="sxs-lookup"><span data-stu-id="84d8b-111">Notes:</span></span>

- <span data-ttu-id="84d8b-112">Vraćanjem na servis OneDrive prekidaju se sve postojeće sinkronizacijske veze (uključujući osobni servis OneDrive ako je postavljen).</span><span class="sxs-lookup"><span data-stu-id="84d8b-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="84d8b-113">Nećete izgubiti datoteke ili podatke tako da ponovno postavite OneDrive na računalu.</span><span class="sxs-lookup"><span data-stu-id="84d8b-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="84d8b-114">**Da biste vratili izvorne postavke servisa OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="84d8b-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="84d8b-115">Otvorite dijaloški okvir Pokreni pritiskom na tipku Sustava Windows i R.</span><span class="sxs-lookup"><span data-stu-id="84d8b-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="84d8b-116">Upišite %localappdata%\Microsoft\OneDrive\onedrive.exe /resetiraj i pritisnite OK.</span><span class="sxs-lookup"><span data-stu-id="84d8b-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="84d8b-117">Može se nakratko pojaviti prozor naredbe.</span><span class="sxs-lookup"><span data-stu-id="84d8b-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="84d8b-118">Ručno pokretanje servisa OneDrive tako da otvorite Start</span><span class="sxs-lookup"><span data-stu-id="84d8b-118">Manually launch OneDrive by going to Start</span></span> ![Pritisnite tipku Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="84d8b-120">, u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.</span><span class="sxs-lookup"><span data-stu-id="84d8b-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="84d8b-121">Bilješke:</span><span class="sxs-lookup"><span data-stu-id="84d8b-121">Notes:</span></span>

- <span data-ttu-id="84d8b-122">Ako ste odabrali sinkronizaciju samo nekih mapa prije ponovnog postavljanja, morat ćete to učiniti ponovno nakon dovršetka sinkronizacije.</span><span class="sxs-lookup"><span data-stu-id="84d8b-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="84d8b-123">Dodatne informacije [potražite u odjeljku Odaberite mape servisa OneDrive za sinkronizaciju s računalom.](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)  </span><span class="sxs-lookup"><span data-stu-id="84d8b-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="84d8b-124">To ćete morati dovršiti za osobne OneDrive i OneDrive za tvrtke.</span><span class="sxs-lookup"><span data-stu-id="84d8b-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>