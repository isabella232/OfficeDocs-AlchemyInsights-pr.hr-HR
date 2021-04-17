---
title: Postavke pokretanja u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828144"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="130a8-102">Postavke pokretanja u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="130a8-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="130a8-103">**Promjena aplikacija koje se automatski pokreće prilikom pokretanja**</span><span class="sxs-lookup"><span data-stu-id="130a8-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="130a8-104">Otvorite [Postavke > aplikacije > Pokretanje](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="130a8-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="130a8-105">Provjerite je li bilo koja aplikacija koju želite pokrenuti prilikom pokretanja **uključena**.</span><span class="sxs-lookup"><span data-stu-id="130a8-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="130a8-106">**Dodavanje aplikacije za automatsko pokretanje prilikom pokretanja**</span><span class="sxs-lookup"><span data-stu-id="130a8-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="130a8-107">Kliknite ili dodirnite **Start** pa pronađite aplikaciju koju želite pokrenuti prilikom pokretanja.</span><span class="sxs-lookup"><span data-stu-id="130a8-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="130a8-108">Desnom tipkom miša kliknite aplikaciju, zatim **Više**, a zatim **Otvori mjesto datoteke**.</span><span class="sxs-lookup"><span data-stu-id="130a8-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="130a8-109">Time se otvara mjesto na koje se sprema prečac do aplikacije.</span><span class="sxs-lookup"><span data-stu-id="130a8-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="130a8-110">Ako nema mogućnosti Za otvaranje mjesta datoteke, to znači da se aplikacija ne može pokrenuti prilikom pokretanja.</span><span class="sxs-lookup"><span data-stu-id="130a8-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="130a8-111">Kada je mjesto datoteke otvoreno, pritisnite tipku s logotipom **sustava Windows + R**, upišite **shell:startup**, a zatim kliknite U **redu**.</span><span class="sxs-lookup"><span data-stu-id="130a8-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="130a8-112">Time se otvara mapa Pokretanje.</span><span class="sxs-lookup"><span data-stu-id="130a8-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="130a8-113">Kopirajte i zalijepite prečac do aplikacije s mjesta datoteke u mapu Polazno.</span><span class="sxs-lookup"><span data-stu-id="130a8-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="130a8-114">**Napredne mogućnosti pokretanja (uključujući siguran način rada, postavke UEFI-ja i pokretanje s drugog uređaja)**</span><span class="sxs-lookup"><span data-stu-id="130a8-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="130a8-115">Spremite svoj rad i zatvorite sve otvorene dokumente jer će se ovim koracima ponovno pokrenuti PC.</span><span class="sxs-lookup"><span data-stu-id="130a8-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="130a8-116">Idite [na Postavke > Ažuriranje & sigurnost > oporavak](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="130a8-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="130a8-117">U **odjeljku Napredno pokretanje** kliknite Odmah ponovno **pokreni**.</span><span class="sxs-lookup"><span data-stu-id="130a8-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="130a8-118">Kada se PC ponovno pokrene na zaslon Odabir mogućnosti:</span><span class="sxs-lookup"><span data-stu-id="130a8-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="130a8-119">Da biste se digli s uređaja kao što je USB pogon, **kliknite Koristi uređaj**.</span><span class="sxs-lookup"><span data-stu-id="130a8-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="130a8-120">Da biste unijeli UEFI postavke (ponekad se nazivaju postavljanjem **BIOS-a), kliknite Otklanjanje poteškoća > dodatne mogućnosti > postavke UEFI opreme**.</span><span class="sxs-lookup"><span data-stu-id="130a8-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="130a8-121">Da biste unijeli sigurni način rada ili promijenili napredne postavke pokretanja, **kliknite Otklanjanje poteškoća > dodatne mogućnosti > postavke pokretanja**, a zatim ponovno **pokreni**.</span><span class="sxs-lookup"><span data-stu-id="130a8-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="130a8-122">Možda će se od vas tražiti da unesete [ključ za oporavak značajke BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="130a8-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="130a8-123">Kada se PC ponovno pokrene, kliknite postavku pokretanja koju želite koristiti.</span><span class="sxs-lookup"><span data-stu-id="130a8-123">After your PC restarts again, click the startup setting you want to use.</span></span>