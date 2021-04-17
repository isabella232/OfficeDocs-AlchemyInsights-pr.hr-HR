---
title: Otklanjanje poteškoća sa servisom OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826191"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="99a4e-102">Otklanjanje poteškoća sa servisom OneDrive</span><span class="sxs-lookup"><span data-stu-id="99a4e-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="99a4e-103">Ako se OneDrive više puta ruši, isprobajte sljedeće korake za otklanjanje poteškoća:</span><span class="sxs-lookup"><span data-stu-id="99a4e-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="99a4e-104">**Provjerite nisu li ključevi registra postavljeni:**</span><span class="sxs-lookup"><span data-stu-id="99a4e-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="99a4e-105">Pomoću uređivača registra idite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="99a4e-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="99a4e-106">Ako je disableFileSyncNGSC prisutan i postavljen na 1, otvorite ključ i promijenite vrijednost u 0.</span><span class="sxs-lookup"><span data-stu-id="99a4e-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="99a4e-107">Ručno pokretanje servisa OneDrive na izborniku Start</span><span class="sxs-lookup"><span data-stu-id="99a4e-107">Manually launch OneDrive by going to Start</span></span> ![Pritiskanje tipke sustava Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="99a4e-109">, u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.</span><span class="sxs-lookup"><span data-stu-id="99a4e-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="99a4e-110">**Ponovno postavljanje servisa OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="99a4e-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="99a4e-111">Napomene:</span><span class="sxs-lookup"><span data-stu-id="99a4e-111">Notes:</span></span>

- <span data-ttu-id="99a4e-112">Ponovno postavljanje servisa OneDrive prekida vezu sa svim postojećim vezama za sinkronizaciju (uključujući osobni OneDrive ako je postavljen).</span><span class="sxs-lookup"><span data-stu-id="99a4e-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="99a4e-113">Nećete izgubiti datoteke ni podatke tako da ponovno na računalu ponovno e-postavljanjem servisa OneDrive.</span><span class="sxs-lookup"><span data-stu-id="99a4e-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="99a4e-114">**Ponovno postavljanje servisa OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="99a4e-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="99a4e-115">Otvorite dijaloški okvir Pokreni pritiskom na tipku Windows i R.</span><span class="sxs-lookup"><span data-stu-id="99a4e-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="99a4e-116">Upišite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset pa pritisnite U redu.</span><span class="sxs-lookup"><span data-stu-id="99a4e-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="99a4e-117">Nakratko se može pojaviti prozor Naredbe.</span><span class="sxs-lookup"><span data-stu-id="99a4e-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="99a4e-118">Ručno pokretanje servisa OneDrive na izborniku Start</span><span class="sxs-lookup"><span data-stu-id="99a4e-118">Manually launch OneDrive by going to Start</span></span> ![Pritiskanje tipke sustava Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="99a4e-120">, u okvir za pretraživanje upišite OneDrive, a zatim kliknite aplikaciju OneDrive za stolna računala.</span><span class="sxs-lookup"><span data-stu-id="99a4e-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="99a4e-121">Napomene:</span><span class="sxs-lookup"><span data-stu-id="99a4e-121">Notes:</span></span>

- <span data-ttu-id="99a4e-122">Ako ste prije vraćanja na izvorno odabrali sinkronizaciju samo nekih mapa, morat ćete to ponoviti kada se sinkronizacija dovrši.</span><span class="sxs-lookup"><span data-stu-id="99a4e-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="99a4e-123">Dodatne [informacije potražite u odabiru mapa servisa OneDrive koje](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)želite   sinkronizirati s računalom.</span><span class="sxs-lookup"><span data-stu-id="99a4e-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="99a4e-124">To ćete morati dovršiti za osobni OneDrive i OneDrive za tvrtke.</span><span class="sxs-lookup"><span data-stu-id="99a4e-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>