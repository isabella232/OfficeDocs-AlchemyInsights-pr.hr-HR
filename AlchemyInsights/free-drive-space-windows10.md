---
title: Oslobađanje prostora na disku u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505348"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="7e6e5-102">Oslobađanje prostora na disku u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="7e6e5-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="7e6e5-103">Evo dvije mogućnosti za oslobađanje prostora na disku u sustavu Windows:</span><span class="sxs-lookup"><span data-stu-id="7e6e5-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="7e6e5-104">Oslobađanje prostora na disku u sustavu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="7e6e5-105">Oslobodite prostor za ažuriranja sustava Windows 10 pomoću vanjskog uređaja za pohranu.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="7e6e5-106">Ako nakon čišćenja diska i dalje imate malo prostora na disku, moguće je da se vaša privremena mapa brzo puni aplikacijskim datotekama (.appx) koje upotrebljava Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="7e6e5-107">Za rješavanje ovog problema ponovo postavite Store, očistite njegovu predmemoriju te pokrenite alat za otklanjanje poteškoća sustava Windows Update.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="7e6e5-108">Provjerite je li Microsoft Store zatvoren prije nego što nastavite s ovim koracima.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="7e6e5-109">**Korak 1: Ponovo postavite Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="7e6e5-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="7e6e5-110">**Napomena** Ovo trajno briše podatke aplikacije na uređaju, uključujući vaše preferencije i pojedinosti o prijavi.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="7e6e5-111">Odaberite **Start** > **Postavke** > **Aplikacije** > **Aplikacije & značajke**.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="7e6e5-112">Na popisu aplikacija pronađite i odaberite Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="7e6e5-113">Odaberite **Dodatne mogućnosti**.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="7e6e5-114">Pomaknite se prema dolje i odaberite **Ponovo postavi**, a zatim **Potvrdi ponovno postavljanje**.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="7e6e5-115">**Korak 2: očisti predmemoriju aplikacije Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="7e6e5-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="7e6e5-116">Pritisnite tipku s logotipom sustava Windows i slovo R da biste otvorili dijaloški okvir Pokreni.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="7e6e5-117">Upišite wsreset.exe i odaberite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="7e6e5-118">Otvara se prazan prozor naredbenog retka.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="7e6e5-119">Nakon otprilike 10 sekundi, prozor se zatvara i Store se automatski otvara.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="7e6e5-120">**Korak 3: ponovo postavite Windows Update**</span><span class="sxs-lookup"><span data-stu-id="7e6e5-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="7e6e5-121">Odaberite **Start** > **Postavke** > **Ažuriranje & Sigurnost** > **Otklanjanje poteškoća**.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="7e6e5-122">Pomaknite se prema dolje i odaberite **Windows Update** s popisa, i odaberite **Pokreni alat za otklanjanje poteškoća**.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="7e6e5-123">Ponovo pokrenite računalo i provjerite pojavljuje li se i dalje problem.</span><span class="sxs-lookup"><span data-stu-id="7e6e5-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

