---
title: Otklanjanje poteškoća s postojećim monitorom
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690703"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="030ea-102">Otklanjanje poteškoća s postojećim monitorom</span><span class="sxs-lookup"><span data-stu-id="030ea-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="030ea-103">Isprobajte ova rješenja da biste otklonili poteškoće s monitorom.</span><span class="sxs-lookup"><span data-stu-id="030ea-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="030ea-104">**Osvježavanje zaslona monitora:**</span><span class="sxs-lookup"><span data-stu-id="030ea-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="030ea-105">Istodobno pritišćite sljedeće tipke: tipka sa sustavom Windows + Ctrl + Shift + B. Time ćete osvježiti komunikaciju s grafičkim upravljačkim programom.</span><span class="sxs-lookup"><span data-stu-id="030ea-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="030ea-106">Monitori će uskoro trepnuti i vratiti se nakon nekoliko sekundi.</span><span class="sxs-lookup"><span data-stu-id="030ea-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="030ea-107">**Otklanjanje poteškoća s hardverom monitora:**</span><span class="sxs-lookup"><span data-stu-id="030ea-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="030ea-108">Isključite kabel koji povezuje PC s monitorom i ponovno ga priključite.</span><span class="sxs-lookup"><span data-stu-id="030ea-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="030ea-109">Isključite sve uređaje koji nisu neophodni na PC-ju (primjerice adaptere ili dokove).</span><span class="sxs-lookup"><span data-stu-id="030ea-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="030ea-110">**Ako ste nedavno instalirali ažuriranje na PC, možete vratiti upravljački program za prikaz:**</span><span class="sxs-lookup"><span data-stu-id="030ea-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="030ea-111">Odaberite **Start**, upišite **Upravitelj uređaja**, a zatim odaberite **Upravitelj uređaja** iz rezultata.</span><span class="sxs-lookup"><span data-stu-id="030ea-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="030ea-112">Proširite odjeljak **prilagodnici prikaza** , desnom tipkom miša kliknite zaslonski prilagodnik, a zatim odaberite **Svojstva**.</span><span class="sxs-lookup"><span data-stu-id="030ea-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="030ea-113">Idite na karticu **upravljački** program, a zatim odaberite **Vratite upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="030ea-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="030ea-114">Pažnja: ako to nije dostupno ili je zasivljeno, odaberite **ne** iz mogućnosti u nastavku da biste se pomaknuli na sljedeći korak.</span><span class="sxs-lookup"><span data-stu-id="030ea-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="030ea-115">Možda ćete morati ponovno pokrenuti PC da bi promjene stupile na ruku.</span><span class="sxs-lookup"><span data-stu-id="030ea-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="030ea-116">**Deinstalirajte i ponovno instalirajte upravljački program za prikaz:**</span><span class="sxs-lookup"><span data-stu-id="030ea-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="030ea-117">Odaberite **Start**, upišite **Upravitelj uređaja**, a zatim odaberite **Upravitelj uređaja** iz rezultata.</span><span class="sxs-lookup"><span data-stu-id="030ea-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="030ea-118">Proširite odjeljak **prilagodnici prikaza** , desnom tipkom miša kliknite zaslonski prilagodnik, a zatim odaberite **Deinstaliraj uređaj**.</span><span class="sxs-lookup"><span data-stu-id="030ea-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="030ea-119">Odaberite okvir uz **gumb Izbriši upravljački program za ovaj uređaj** i odaberite **Deinstaliraj**.</span><span class="sxs-lookup"><span data-stu-id="030ea-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="030ea-120">Pažnja: u ovoj će se fazi možda zatražiti da ponovno pokrenete računalo.</span><span class="sxs-lookup"><span data-stu-id="030ea-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="030ea-121">Prije ponovnog pokretanja obavezno zapišite preostale upute.</span><span class="sxs-lookup"><span data-stu-id="030ea-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="030ea-122">Ponovno otvorite upravitelj uređaja.</span><span class="sxs-lookup"><span data-stu-id="030ea-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="030ea-123">Proširite odjeljak **prilagodnici prikaza** , desnom tipkom miša kliknite zaslonski prilagodnik, a zatim odaberite **Ažuriraj upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="030ea-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="030ea-124">Odaberite **Pretraživanje automatski radi ažuriranja upravljačkih** programa i slijedite upute za instalaciju.</span><span class="sxs-lookup"><span data-stu-id="030ea-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>