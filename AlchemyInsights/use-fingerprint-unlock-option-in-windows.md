---
title: Korištenje mogućnosti otključavanja otisaka prstiju u sustavu Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795236"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="8afcc-102">Korištenje mogućnosti otključavanja otisaka prstiju u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="8afcc-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="8afcc-103">**Omogućivanje otiska prsta u sustavu Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="8afcc-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="8afcc-104">Da biste otključali Windows 10 pomoću otiska prsta, morate postaviti otisak prsta u sustavu Windows Hello dodavanjem (ostavljajući Windows da sazna da prepozna) barem jedan prst.</span><span class="sxs-lookup"><span data-stu-id="8afcc-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="8afcc-105">Idite na **postavke > računi > mogućnosti prijave** (ili kliknite [ovdje](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="8afcc-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="8afcc-106">Dostupne mogućnosti prijave prikazat će se na popisu.</span><span class="sxs-lookup"><span data-stu-id="8afcc-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="8afcc-107">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="8afcc-107">For example:</span></span>

    ![Mogućnosti prijave](media/sign-in-options.png)

2. <span data-ttu-id="8afcc-109">Kliknite ili dodirnite **otisak prsta u sustavu Windows Hello**, a zatim kliknite **Postavi**.</span><span class="sxs-lookup"><span data-stu-id="8afcc-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="8afcc-110">U prozoru Postavljanje sustava Windows Hello kliknite **početak rada**.</span><span class="sxs-lookup"><span data-stu-id="8afcc-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="8afcc-111">Senzor otiska prsta aktivirat će se i od vas će se zatražiti da postavite prst na senzor:</span><span class="sxs-lookup"><span data-stu-id="8afcc-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor otisaka prstiju.](media/fingerprint-sensor.png)

3. <span data-ttu-id="8afcc-113">Slijedite upute koje će vas upitati da opetovano skenirate prst.</span><span class="sxs-lookup"><span data-stu-id="8afcc-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="8afcc-114">Kada ovo završite, imat ćete mogućnost dodavanja drugih prstiju koje želite koristiti za prijavu.</span><span class="sxs-lookup"><span data-stu-id="8afcc-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="8afcc-115">Kada se sljedeći put prijavite u Windows 10, imat ćete mogućnost korištenja otiska prsta da biste to učinili.</span><span class="sxs-lookup"><span data-stu-id="8afcc-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="8afcc-116">**Otisak prsta u sustavu Windows Hello nije dostupan kao mogućnost prijave**</span><span class="sxs-lookup"><span data-stu-id="8afcc-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="8afcc-117">Ako se otisci zaslona u sustavu Windows Hello ne prikazuju kao mogućnost u **mogućnostima prijave**, znači da Windows nije svjestan bilo kojeg čitača otisaka prstiju koji je priključen na PC ili da pravilnik sustava sprječava njegovo korištenje (ako na PC-ju upravlja vaše radno mjesto).</span><span class="sxs-lookup"><span data-stu-id="8afcc-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="8afcc-118">Otklanjanje poteškoća:</span><span class="sxs-lookup"><span data-stu-id="8afcc-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="8afcc-119">Odaberite gumb **Start** na programskoj traci i potražite **upravitelja uređaja**.</span><span class="sxs-lookup"><span data-stu-id="8afcc-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="8afcc-120">Kliknite ili dodirnite da biste otvorili **Upravitelj uređaja**.</span><span class="sxs-lookup"><span data-stu-id="8afcc-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="8afcc-121">U upravitelju uređaja proširite Biometrijski uređaji tako da kliknete njegov Chevron.</span><span class="sxs-lookup"><span data-stu-id="8afcc-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrijskih uređaja.](media/biometric-devices.png)

4. <span data-ttu-id="8afcc-123">Skener otisaka prstiju trebao bi biti naveden kao biometrijski uređaj, kao što je sinaptički WBDI Scanner:</span><span class="sxs-lookup"><span data-stu-id="8afcc-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrijskih uređaja.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="8afcc-125">Ako vam se ne prikaže skener otisaka prstiju, a skener je integriran na PC, otvorite web-mjesto proizvođača PC-ja.</span><span class="sxs-lookup"><span data-stu-id="8afcc-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="8afcc-126">U odjeljku tehnička podrška za PC model potražite upravljački program za Windows 10 za skener koji možete instalirati.</span><span class="sxs-lookup"><span data-stu-id="8afcc-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="8afcc-127">Ako je skener odvojen od PC-ja (priključen putem USB-a), otvorite web-mjesto proizvođača skenera da biste pronašli i instalirali upravljački program za uređaj sa sustavom Windows 10 za model skenera koji imate.</span><span class="sxs-lookup"><span data-stu-id="8afcc-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
