---
title: Nedostaje ikona napajanja ili baterije u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: d82994c86126ea9c789e846a74e03794c32c5c3c
ms.sourcegitcommit: b398afd92d4259f893c25b48aec65921e6cc68d6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/16/2020
ms.locfileid: "44269011"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="19e37-102">Nedostaje ikona napajanja ili baterije u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="19e37-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="19e37-103">Ako vaš uređaj sa sustavom Windows 10 ima bateriju (npr. prijenosno računalo ili tablet ili PC povezan putem USB-a s UPS-om), obično se ikona napajanja/baterije prikazuje na programskoj traci blizu sata, na primjer:</span><span class="sxs-lookup"><span data-stu-id="19e37-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Ikona baterije](media/battery-icon.png)

<span data-ttu-id="19e37-105">Ako ne vidite ovu ikonu, možda je skrivena:</span><span class="sxs-lookup"><span data-stu-id="19e37-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="19e37-106">Idite na **[> programsk >a traka za prilagodbu postavki](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="19e37-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="19e37-107">U području Obavijesti kliknite **Odaberi ikone koje će se pojaviti na programskoj traci**.</span><span class="sxs-lookup"><span data-stu-id="19e37-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="19e37-108">Zatim pronađite stavku **Napajanje** na popisu i prebacite njegovu postavku na **Uključeno**.</span><span class="sxs-lookup"><span data-stu-id="19e37-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Prikaži ikonu napajanja na programskoj traci](media/power-icon-on.png)

<span data-ttu-id="19e37-110">**Otklanjanje poteškoća**</span><span class="sxs-lookup"><span data-stu-id="19e37-110">**Troubleshooting**</span></span>

<span data-ttu-id="19e37-111">Ako ste slijedili gore navedene upute, a prekidač **za napajanje** zasivljen je ili nije vidljiv, u okvir za pretraživanje na programskoj traci upišite **upravitelj uređaja,** a zatim na popisu rezultata odaberite **Upravitelj uređaja.**</span><span class="sxs-lookup"><span data-stu-id="19e37-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="19e37-112">U **odjeljku Baterije**desnom tipkom miša kliknite bateriju uređaja, kliknite **Onemogući**, a zatim **Da**.</span><span class="sxs-lookup"><span data-stu-id="19e37-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="19e37-113">Pričekajte nekoliko sekundi, a zatim desnom tipkom miša kliknite bateriju i kliknite **Omogući**.</span><span class="sxs-lookup"><span data-stu-id="19e37-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="19e37-114">Zatim ponovno pokrenite uređaj.</span><span class="sxs-lookup"><span data-stu-id="19e37-114">Then restart your device.</span></span>

<span data-ttu-id="19e37-115">Ako ste slijedili gore navedene upute, ali se ikona baterije ne pojavljuje na programskoj traci, u okvir za pretraživanje na programskoj traci upišite **upravitelj zadataka,** a zatim na popisu rezultata kliknite **Upravitelj zadataka.**</span><span class="sxs-lookup"><span data-stu-id="19e37-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="19e37-116">Na kartici **Procesi** u odjeljku **Naziv**desnom tipkom miša kliknite **Explorer**, a zatim kliknite **Ponovno pokreni**.</span><span class="sxs-lookup"><span data-stu-id="19e37-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
