---
title: Otklanjanje poteškoća s postojećim monitorom
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824571"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="93a6c-102">Otklanjanje poteškoća s postojećim monitorom</span><span class="sxs-lookup"><span data-stu-id="93a6c-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="93a6c-103">Isprobajte ova rješenja da biste otklonili poteškoće s monitorom.</span><span class="sxs-lookup"><span data-stu-id="93a6c-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="93a6c-104">**Osvježite zaslon monitora:**</span><span class="sxs-lookup"><span data-stu-id="93a6c-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="93a6c-105">Istodobno pritišćite sljedeće tipke: Tipka windows + Ctrl + Shift + B. Time ćete osvježiti komunikaciju s upravljačkim programom za grafiku.</span><span class="sxs-lookup"><span data-stu-id="93a6c-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="93a6c-106">Monitori će trenuci treptati i vratiti se nakon nekoliko sekundi.</span><span class="sxs-lookup"><span data-stu-id="93a6c-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="93a6c-107">**Otklanjanje poteškoća s hardverom monitora:**</span><span class="sxs-lookup"><span data-stu-id="93a6c-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="93a6c-108">Isključite kabel koji povezuje PC s monitorom i ponovno ga priključite.</span><span class="sxs-lookup"><span data-stu-id="93a6c-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="93a6c-109">Odspojite sve uređaje koji nisu ključni s PC-ja (kao što su prilagodnici ili sidrišta).</span><span class="sxs-lookup"><span data-stu-id="93a6c-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="93a6c-110">**Ako ste nedavno instalirali ažuriranje na PC, možete vratiti upravljački program za prikaz:**</span><span class="sxs-lookup"><span data-stu-id="93a6c-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="93a6c-111">Odaberite **Start**, **upišite upravitelj uređaja**, a **zatim u rezultatima** odaberite Upravitelj uređaja.</span><span class="sxs-lookup"><span data-stu-id="93a6c-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="93a6c-112">Proširite **odjeljak Prilagodnici** za prikaz, desnom tipkom miša kliknite prilagodnik za prikaz, a zatim odaberite **Svojstva**.</span><span class="sxs-lookup"><span data-stu-id="93a6c-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="93a6c-113">Pomaknite se do **kartice Upravljački** program i **odaberite Vrati upravljački program .**</span><span class="sxs-lookup"><span data-stu-id="93a6c-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="93a6c-114">Napomena: ako to nije dostupno ili je  zasivljeno, na mogućnostima u nastavku odaberite Ne da biste se pomakli na sljedeći korak.</span><span class="sxs-lookup"><span data-stu-id="93a6c-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="93a6c-115">Prije nego što te promjene stupe na snagu, možda ćete morati ponovno pokrenuti PC.</span><span class="sxs-lookup"><span data-stu-id="93a6c-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="93a6c-116">**Deinstalirajte i ponovno instalirajte upravljački program za prikaz:**</span><span class="sxs-lookup"><span data-stu-id="93a6c-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="93a6c-117">Odaberite **Start**, **upišite upravitelj uređaja**, a **zatim u rezultatima** odaberite Upravitelj uređaja.</span><span class="sxs-lookup"><span data-stu-id="93a6c-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="93a6c-118">Proširite **odjeljak Prilagodnici za** prikaz, desnom tipkom miša kliknite prilagodnik za prikaz, a zatim odaberite **Deinstaliraj uređaj**.</span><span class="sxs-lookup"><span data-stu-id="93a6c-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="93a6c-119">Odaberite okvir uz stavku **Brisanje upravljačkog softvera za ovaj uređaj i odaberite** **Deinstaliraj**.</span><span class="sxs-lookup"><span data-stu-id="93a6c-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="93a6c-120">Napomena: od vas će se možda tražiti da ponovno pokrenete računalo u ovoj fazi.</span><span class="sxs-lookup"><span data-stu-id="93a6c-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="93a6c-121">Prije ponovnog pokretanja obavezno zapišite preostale upute.</span><span class="sxs-lookup"><span data-stu-id="93a6c-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="93a6c-122">Ponovno otvorite Upravitelj uređaja.</span><span class="sxs-lookup"><span data-stu-id="93a6c-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="93a6c-123">Proširite odjeljak **Prilagodnici za** prikaz, desnom tipkom miša kliknite prilagodnik za prikaz, a zatim odaberite **Ažuriraj upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="93a6c-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="93a6c-124">Odaberite **Automatski traži softver za ažuriranje upravljačkog programa** i slijedite upute za instalaciju.</span><span class="sxs-lookup"><span data-stu-id="93a6c-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>