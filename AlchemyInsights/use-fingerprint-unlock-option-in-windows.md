---
title: Mogućnost otključavanja otiskom prsta u sustavu Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796669"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="8fad6-102">Mogućnost otključavanja otiskom prsta u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="8fad6-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="8fad6-103">**Omogućivanje otiska prsta u sustavu Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="8fad6-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="8fad6-104">Da biste otključali Windows 10 pomoću otiska prsta, morate postaviti otisak prsta značajke Windows Hello tako da dodate (ostavljajući sustavu Windows da nauči prepoznati) barem jedan prst.</span><span class="sxs-lookup"><span data-stu-id="8fad6-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="8fad6-105">Otvorite **Postavke > računi > mogućnosti prijave** (ili kliknite [ovdje).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="8fad6-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="8fad6-106">Na popisu će biti dostupne mogućnosti prijave.</span><span class="sxs-lookup"><span data-stu-id="8fad6-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="8fad6-107">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="8fad6-107">For example:</span></span>

    ![Mogućnosti prijave.](media/sign-in-options.png)

2. <span data-ttu-id="8fad6-109">Kliknite ili dodirnite **Otisak prsta značajke Windows Hello**, a zatim **Postavi**.</span><span class="sxs-lookup"><span data-stu-id="8fad6-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="8fad6-110">U prozoru za postavljanje značajke Windows Hello **kliknite Početak rada**.</span><span class="sxs-lookup"><span data-stu-id="8fad6-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="8fad6-111">Aktivirat će se senzor otiska prsta i od vas će se tražiti da postavite prst na senzor:</span><span class="sxs-lookup"><span data-stu-id="8fad6-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor otiska prsta.](media/fingerprint-sensor.png)

3. <span data-ttu-id="8fad6-113">Slijedite upute koje će od vas tražiti da više puta skenirate prst.</span><span class="sxs-lookup"><span data-stu-id="8fad6-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="8fad6-114">Kada to završite, možete dodati i druge prste koje biste mogli koristiti za prijavu.</span><span class="sxs-lookup"><span data-stu-id="8fad6-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="8fad6-115">Kada se sljedeći put prijavite u Windows 10, za to ćete imati mogućnost korištenja otiska prsta.</span><span class="sxs-lookup"><span data-stu-id="8fad6-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="8fad6-116">**Windows Hello Fingerprint not available as a sign-in option**</span><span class="sxs-lookup"><span data-stu-id="8fad6-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="8fad6-117">Ako se u mogućnostima prijave ne prikazuje otisak prsta u sustavu Windows Hello **,** to znači da Windows nije upoznat s čitačem otisaka prstiju/skenerom priloženim na PC-ju ili da pravilnik sustava sprječava njegovo korištenje (ako, primjerice, računalom upravlja vaše radno mjesto).</span><span class="sxs-lookup"><span data-stu-id="8fad6-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="8fad6-118">Da biste otklonili poteškoće:</span><span class="sxs-lookup"><span data-stu-id="8fad6-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="8fad6-119">Odaberite **gumb Start** na programskoj traci i potražite Upravitelj **uređaja**.</span><span class="sxs-lookup"><span data-stu-id="8fad6-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="8fad6-120">Kliknite ili dodirnite da biste **otvorili Upravitelj uređaja**.</span><span class="sxs-lookup"><span data-stu-id="8fad6-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="8fad6-121">U upravitelju uređaja proširite Biometrijske uređaje klikom na ševron.</span><span class="sxs-lookup"><span data-stu-id="8fad6-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrijski uređaji.](media/biometric-devices.png)

4. <span data-ttu-id="8fad6-123">Skener otiska prsta trebao bi biti naveden kao biometrijski uređaj, kao što je synaptics WBDI skener:</span><span class="sxs-lookup"><span data-stu-id="8fad6-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrijski uređaji.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="8fad6-125">Ako se skener otiska prsta ne prikazuje, a skener je integriran u PC, idite na web-mjesto proizvođača PC-ja.</span><span class="sxs-lookup"><span data-stu-id="8fad6-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="8fad6-126">U odjeljku tehničke podrške za model PC-ja potražite upravljački program za Windows 10 za skener koji možete instalirati.</span><span class="sxs-lookup"><span data-stu-id="8fad6-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="8fad6-127">Ako je skener odvojen od PC-ja (priložen putem USB-a), idite na web-mjesto proizvođača skenera da biste pronašli i instalirali softver za upravljačke programe uređaja sa sustavom Windows 10 za model skenera koji imate.</span><span class="sxs-lookup"><span data-stu-id="8fad6-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
