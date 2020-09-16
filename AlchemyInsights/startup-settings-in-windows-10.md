---
title: Postavke pokretanja u sustavu Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751127"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="1709a-102">Postavke pokretanja u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="1709a-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="1709a-103">**Promjena aplikacija koje se automatski pokreću prilikom pokretanja**</span><span class="sxs-lookup"><span data-stu-id="1709a-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="1709a-104">Idite na [postavke > aplikacije > Startup](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="1709a-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="1709a-105">Provjerite je **li uključena bilo**koja aplikacija koju želite pokrenuti pri pokretanju.</span><span class="sxs-lookup"><span data-stu-id="1709a-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="1709a-106">**Dodavanje aplikacije koja će se automatski pokretati prilikom pokretanja**</span><span class="sxs-lookup"><span data-stu-id="1709a-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="1709a-107">Kliknite ili dodirnite **Start** , a zatim pronađite aplikaciju koju želite pokrenuti prilikom pokretanja.</span><span class="sxs-lookup"><span data-stu-id="1709a-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="1709a-108">Desnom tipkom miša kliknite aplikaciju, kliknite **više**, a zatim **Otvori mjesto datoteke**.</span><span class="sxs-lookup"><span data-stu-id="1709a-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="1709a-109">Time se otvara mjesto na kojem se sprema prečac do aplikacije.</span><span class="sxs-lookup"><span data-stu-id="1709a-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="1709a-110">Ako ne postoji mogućnost otvaranja lokacije datoteke, to znači da se aplikacija ne može pokrenuti prilikom pokretanja.</span><span class="sxs-lookup"><span data-stu-id="1709a-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="1709a-111">Ako je mjesto datoteke otvoreno, pritisnite **tipku s logotipom sustava Windows + R**, upišite **Shell: Startup**( **u redu**).</span><span class="sxs-lookup"><span data-stu-id="1709a-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="1709a-112">Time se otvara mapa Startup (Polazno).</span><span class="sxs-lookup"><span data-stu-id="1709a-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="1709a-113">Kopirajte i zalijepite prečac do aplikacije s mjesta datoteke u mapu Startup (Polazno).</span><span class="sxs-lookup"><span data-stu-id="1709a-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="1709a-114">**Napredne mogućnosti pokretanja (uključujući siguran način rada, postavke UEFI-a i dizanje s drugog uređaja)**</span><span class="sxs-lookup"><span data-stu-id="1709a-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="1709a-115">Spremite svoj rad i Zatvori sve otvorene dokumente jer će ti koraci ponovno pokrenuti PC.</span><span class="sxs-lookup"><span data-stu-id="1709a-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="1709a-116">Idite na [postavke > ažuriranje & sigurnosnog > oporavka](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="1709a-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="1709a-117">U odjeljku **Napredno pokretanje**kliknite **Ponovno pokreni sada**.</span><span class="sxs-lookup"><span data-stu-id="1709a-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="1709a-118">Kada se PC ponovno pokrene, odaberite zaslon mogućnosti:</span><span class="sxs-lookup"><span data-stu-id="1709a-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="1709a-119">Da biste se pokrenuti s uređaja kao što je USB pogon, kliknite **koristi uređaj**.</span><span class="sxs-lookup"><span data-stu-id="1709a-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="1709a-120">Da biste unijeli postavke UEFI-a (ponekad se naziva Postavljanje BIOS-a), kliknite **Otklanjanje poteškoća > dodatnim mogućnostima > postavke firmware**-a.</span><span class="sxs-lookup"><span data-stu-id="1709a-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="1709a-121">Da biste unijeli siguran način rada ili promijenili napredne postavke pokretanja, kliknite **Otklanjanje poteškoća > dodatnim mogućnostima > postavke pokretanja**, a zatim **Ponovno pokreni**.</span><span class="sxs-lookup"><span data-stu-id="1709a-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="1709a-122">Možda će se od vas zatražiti da unesete [BitLocker ključ oporavka](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="1709a-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="1709a-123">Nakon ponovnog pokretanja PC-ja kliknite postavku pokretanja koju želite koristiti.</span><span class="sxs-lookup"><span data-stu-id="1709a-123">After your PC restarts again, click the startup setting you want to use.</span></span>