---
title: U sustavu Windows 10 nema ikone napajanja ili baterije
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790540"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="f485c-102">U sustavu Windows 10 nema ikone napajanja ili baterije</span><span class="sxs-lookup"><span data-stu-id="f485c-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="f485c-103">Ako uređaj sa sustavom Windows 10 ima bateriju (npr. prijenosno računalo, tablet ili PC povezan s UPS-om putem USB-a), obično se na programskoj traci u blizini sata prikazuje ikona napajanja/baterije, na primjer:</span><span class="sxs-lookup"><span data-stu-id="f485c-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Ikona baterije](media/battery-icon.png)

<span data-ttu-id="f485c-105">Ako ne vidite tu ikonu, možda je skrivena:</span><span class="sxs-lookup"><span data-stu-id="f485c-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="f485c-106">Otvorite **[Postavke > Personalizacija > Programska traka](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="f485c-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="f485c-107">U području obavijesti kliknite mogućnost **Odaberite koje će se ikone prikazivati na programskoj traci**.</span><span class="sxs-lookup"><span data-stu-id="f485c-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="f485c-108">Potom na popisu pronađite stavku **Napajanje** i prebacite njezinu postavku na **Uključeno**.</span><span class="sxs-lookup"><span data-stu-id="f485c-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Prikaži ikonu napajanja na programskoj traci](media/power-icon-on.png)

<span data-ttu-id="f485c-110">**Otklanjanje poteškoća**</span><span class="sxs-lookup"><span data-stu-id="f485c-110">**Troubleshooting**</span></span>

<span data-ttu-id="f485c-111">Ako ste slijedili navedene upute, ali je prekidač **Napajanje** zasivljen ili nije vidljiv, u okvir za pretraživanje na programskoj traci upišite **upravitelj uređaja**, a zatim na popisu rezultata odaberite **Upravitelj uređaja**.</span><span class="sxs-lookup"><span data-stu-id="f485c-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="f485c-112">U odjeljku **Baterije**, desnom tipkom miša kliknite bateriju svojeg uređaja te kliknite **Onemogući**, a zatim **Da**.</span><span class="sxs-lookup"><span data-stu-id="f485c-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="f485c-113">Pričekajte nekoliko sekundi pa desnom tipkom miša kliknite bateriju, a zatim **Omogući**.</span><span class="sxs-lookup"><span data-stu-id="f485c-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="f485c-114">Potom ponovno pokrenite uređaj.</span><span class="sxs-lookup"><span data-stu-id="f485c-114">Then restart your device.</span></span>

<span data-ttu-id="f485c-115">Ako ste slijedili navedene upute, ali se ikona baterije ne prikazuje na programskoj traci, u okvir za pretraživanje na programskoj traci upišite **upravitelj zadataka**, a zatim na popisu rezultata kliknite **Upravitelj zadataka**.</span><span class="sxs-lookup"><span data-stu-id="f485c-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="f485c-116">Na kartici **Procesi** u odjeljku **Naziv** desnom tipkom miša kliknite **Explorer**, a zatim **Ponovno pokreni**.</span><span class="sxs-lookup"><span data-stu-id="f485c-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
