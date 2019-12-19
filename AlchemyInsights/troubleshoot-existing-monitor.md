---
title: Otklanjanje poteškoća s postojećim monitorom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738561"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="bb330-102">Otklanjanje poteškoća s postojećim monitorom</span><span class="sxs-lookup"><span data-stu-id="bb330-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="bb330-103">Isprobajte ova rješenja za otklanjanje poteškoća s monitorom.</span><span class="sxs-lookup"><span data-stu-id="bb330-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="bb330-104">**Osvježavanje zaslona monitora:**</span><span class="sxs-lookup"><span data-stu-id="bb330-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="bb330-105">Pritisnite sljedeće tipke u isto vrijeme: Windows Key + Ctrl + Shift + B. To će osvježiti komunikaciju s vašim upravljačkim programom za grafiku.</span><span class="sxs-lookup"><span data-stu-id="bb330-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="bb330-106">Vaši monitori će uskoro treptati i vratiti se nakon nekoliko sekundi.</span><span class="sxs-lookup"><span data-stu-id="bb330-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="bb330-107">**Otklanjanje poteškoća s hardverom monitora:**</span><span class="sxs-lookup"><span data-stu-id="bb330-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="bb330-108">Isključite kabel koji povezuje računalo s monitorom i ponovno ga priključite.</span><span class="sxs-lookup"><span data-stu-id="bb330-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="bb330-109">Isključite sve uređaje koji nisu bitni s PC-ja (kao što su adapteri ili dokovi).</span><span class="sxs-lookup"><span data-stu-id="bb330-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="bb330-110">**Ako ste nedavno instalirali ažuriranje na PC-ju, možete vratiti upravljački program za prikaz:**</span><span class="sxs-lookup"><span data-stu-id="bb330-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="bb330-111">Odaberite **Start**, upišite **Upravitelj uređaja**i odaberite **Upravitelj uređaja** iz rezultata.</span><span class="sxs-lookup"><span data-stu-id="bb330-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="bb330-112">Proširite odjeljak **adapteri za prikaz** , desnom tipkom miša kliknite svoj zaslonski prilagodnik, ands odaberite **Svojstva**.</span><span class="sxs-lookup"><span data-stu-id="bb330-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="bb330-113">Prijeđite na karticu **upravljački program** i odaberite **Vrati upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="bb330-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="bb330-114">Napomena: ako to nije dostupno ili je sive vrste, odaberite **ne** iz opcija u nastavku za pomicanje na sljedeći korak.</span><span class="sxs-lookup"><span data-stu-id="bb330-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="bb330-115">Možda ćete morati ponovo pokrenuti PC prije nego što te promjene stupit na snagu.</span><span class="sxs-lookup"><span data-stu-id="bb330-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="bb330-116">**Deinstalirajte i ponovno instalirajte upravljački program za prikaz:**</span><span class="sxs-lookup"><span data-stu-id="bb330-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="bb330-117">Odaberite **Start**, upišite **Upravitelj uređaja**i odaberite **Upravitelj uređaja** iz rezultata.</span><span class="sxs-lookup"><span data-stu-id="bb330-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="bb330-118">Proširite odjeljak **adapteri za prikaz** , desnom tipkom miša kliknite svoj zaslonski prilagodnik, ands odaberite **Deinstaliraj uređaj**.</span><span class="sxs-lookup"><span data-stu-id="bb330-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="bb330-119">Odaberite okvir uz **Brisanje upravljačkog programa za ovaj uređaj** i odaberite **Deinstaliraj**.</span><span class="sxs-lookup"><span data-stu-id="bb330-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="bb330-120">Bilješka: Možda će se od vas tražiti da ponovo pokrenete računalo u ovoj fazi.</span><span class="sxs-lookup"><span data-stu-id="bb330-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="bb330-121">Obavezno zapišite preostale upute prije ponovnog pokretanja.</span><span class="sxs-lookup"><span data-stu-id="bb330-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="bb330-122">Ponovno otvorite upravitelj uređaja.</span><span class="sxs-lookup"><span data-stu-id="bb330-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="bb330-123">Proširite odjeljak **adapteri za prikaz** , desnom tipkom miša kliknite zaslonski prilagodnik i odaberite **Ažuriraj upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="bb330-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="bb330-124">Odaberite **automatski Pretraži za ažuriranje upravljačkog programa** i slijedite upute za instalaciju.</span><span class="sxs-lookup"><span data-stu-id="bb330-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>