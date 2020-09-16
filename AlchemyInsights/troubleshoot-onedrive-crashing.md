---
title: Otklanjanje poteškoća s prekidima servisa OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664990"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="d78e3-102">Otklanjanje poteškoća s prekidima servisa OneDrive</span><span class="sxs-lookup"><span data-stu-id="d78e3-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="d78e3-103">Ako se OneDrive opetovano ruši, isprobajte ove korake za otklanjanje poteškoća:</span><span class="sxs-lookup"><span data-stu-id="d78e3-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="d78e3-104">**Provjerite nisu li postavljeni ključevi registra:**</span><span class="sxs-lookup"><span data-stu-id="d78e3-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="d78e3-105">Pomoću uređivača registra dođite do HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="d78e3-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="d78e3-106">Ako je prisutan DisableFileSyncNGSC i postavljen na 1, otvorite ključ i promijenite vrijednost u 0.</span><span class="sxs-lookup"><span data-stu-id="d78e3-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="d78e3-107">Ručno pokretanje servisa OneDrive tako da počnete s pokretanjem</span><span class="sxs-lookup"><span data-stu-id="d78e3-107">Manually launch OneDrive by going to Start</span></span> ![Pritišćite tipku sa sustavom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="d78e3-109">u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.</span><span class="sxs-lookup"><span data-stu-id="d78e3-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="d78e3-110">**Ponovno postavljanje servisa OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="d78e3-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="d78e3-111">Bilješke</span><span class="sxs-lookup"><span data-stu-id="d78e3-111">Notes:</span></span>

- <span data-ttu-id="d78e3-112">Ponovnim postavljanjem servisa OneDrive prekida se sve postojeće Sinkronizacijske veze (uključujući osobni OneDrive ako je postavljeno).</span><span class="sxs-lookup"><span data-stu-id="d78e3-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="d78e3-113">Datoteke i podatke nećete izgubiti ponovnim postavljanjem servisa OneDrive na računalu.</span><span class="sxs-lookup"><span data-stu-id="d78e3-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="d78e3-114">**Da biste ponovno postavili OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="d78e3-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="d78e3-115">Otvorite dijaloški okvir Pokreni tako da pritisnete tipku sustava Windows i R.</span><span class="sxs-lookup"><span data-stu-id="d78e3-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="d78e3-116">Upišite% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset i pritisnite u redu.</span><span class="sxs-lookup"><span data-stu-id="d78e3-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="d78e3-117">Naredbeni se prozor može pojaviti kratko.</span><span class="sxs-lookup"><span data-stu-id="d78e3-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="d78e3-118">Ručno pokretanje servisa OneDrive tako da počnete s pokretanjem</span><span class="sxs-lookup"><span data-stu-id="d78e3-118">Manually launch OneDrive by going to Start</span></span> ![Pritišćite tipku sa sustavom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="d78e3-120">u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.</span><span class="sxs-lookup"><span data-stu-id="d78e3-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="d78e3-121">Bilješke</span><span class="sxs-lookup"><span data-stu-id="d78e3-121">Notes:</span></span>

- <span data-ttu-id="d78e3-122">Ako ste odabrali sinkronizaciju samo nekih mapa prije ponovnog postavljanja, morat ćete to učiniti ponovno nakon dovršetka sinkronizacije.</span><span class="sxs-lookup"><span data-stu-id="d78e3-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="d78e3-123">Dodatne informacije potražite u odjeljku [Odabir mapa servisa OneDrive za sinkronizaciju s računalom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .</span><span class="sxs-lookup"><span data-stu-id="d78e3-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="d78e3-124">To ćete morati dovršiti radi osobnog servisa OneDrive i servisa OneDrive za tvrtke.</span><span class="sxs-lookup"><span data-stu-id="d78e3-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>