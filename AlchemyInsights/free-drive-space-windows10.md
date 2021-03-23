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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035217"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="438b0-102">Oslobađanje prostora na disku u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="438b0-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="438b0-103">Postoje dvije mogućnosti za oslobađanje prostora na disku u sustavu Windows:</span><span class="sxs-lookup"><span data-stu-id="438b0-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="438b0-104">Oslobodite prostora na disku u sustavu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="438b0-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="438b0-105">Oslobodite prostor za ažuriranja sustava Windows 10 s vanjskim uređajem za pohranu.</span><span class="sxs-lookup"><span data-stu-id="438b0-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="438b0-106">Ako i dalje imate nisko diskovni razmak nakon korištenja značajke čišćenja diska, moguće je da se mapa TEMP brzo ispunjava pomoću datoteka aplikacije (. Appx) koju koristi Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="438b0-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="438b0-107">Da biste riješili taj problem, ponovno postavite trgovinu, poništite predmemoriranje pohrane, a zatim pokrenite alat za otklanjanje poteškoća sa servisom Windows Update.</span><span class="sxs-lookup"><span data-stu-id="438b0-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="438b0-108">Provjerite je li Microsoft Store zatvoren prije nastavka ovih koraka.</span><span class="sxs-lookup"><span data-stu-id="438b0-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="438b0-109">**Prvi korak: ponovno postavljanje Microsoftove trgovine**</span><span class="sxs-lookup"><span data-stu-id="438b0-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="438b0-110">**Notes** Time se trajno brišu podaci o aplikaciji na uređaju, uključujući vaše preference i pojedinosti o prijavi.</span><span class="sxs-lookup"><span data-stu-id="438b0-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="438b0-111">Odaberite **Započni**  >  **Postavke**  >  **aplikacija za aplikacije**  >  **& značajki**.</span><span class="sxs-lookup"><span data-stu-id="438b0-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="438b0-112">Na popisu aplikacija pronađite i odaberite Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="438b0-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="438b0-113">Odaberite **Dodatne mogućnosti**.</span><span class="sxs-lookup"><span data-stu-id="438b0-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="438b0-114">Pomaknite se prema dolje pa odaberite **ponovno postavi**, a zatim **potvrdite ponovno postavi**.</span><span class="sxs-lookup"><span data-stu-id="438b0-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="438b0-115">**Drugi korak: poništite predmemoriranje Microsoftove trgovine**</span><span class="sxs-lookup"><span data-stu-id="438b0-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="438b0-116">Pritisnite tipku s logotipom sustava Windows + R da biste otvorili dijaloški okvir Pokreni.</span><span class="sxs-lookup"><span data-stu-id="438b0-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="438b0-117">Upišite wsreset.exe i odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="438b0-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="438b0-118">Otvorit će se prazan prozor naredbenog upita.</span><span class="sxs-lookup"><span data-stu-id="438b0-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="438b0-119">Nakon približno 10 sekundi prozor će se zatvoriti, a trgovina će se automatski otvoriti.</span><span class="sxs-lookup"><span data-stu-id="438b0-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="438b0-120">**Treći korak: ponovno postavljanje servisa Windows Update**</span><span class="sxs-lookup"><span data-stu-id="438b0-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="438b0-121">Odaberite **Započni**  >    >  **Ažuriranje postavki & sigurnosnim**  >  **otklanjanjem poteškoća**.</span><span class="sxs-lookup"><span data-stu-id="438b0-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="438b0-122">Pomaknite se prema dolje pa na popisu odaberite **Windows Update** , a zatim **Pokrenite alat za otklanjanje poteškoća**.</span><span class="sxs-lookup"><span data-stu-id="438b0-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="438b0-123">Ponovno pokrenite računalo i provjerite jeste li još uvijek doživjeli problem.</span><span class="sxs-lookup"><span data-stu-id="438b0-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

