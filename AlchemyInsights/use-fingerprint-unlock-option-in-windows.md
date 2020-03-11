---
title: Korištenje mogućnosti otključavanja otiska prsta u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588308"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="6dd6b-102">Korištenje mogućnosti otključavanja otiska prsta u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="6dd6b-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="6dd6b-103">**Omogući otisak prsta za pozdrave u sustavu Windows**</span><span class="sxs-lookup"><span data-stu-id="6dd6b-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="6dd6b-104">Da biste otključali Windows 10 pomoću otiska prsta, otisak prsta za Pozdrav sustavom Windows morate postaviti tako da dodate (omogućujući sustavu Windows da nauči prepoznati) barem jedan prst.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="6dd6b-105">Idite na **Postavke > Računi > Mogućnosti prijave** (ili kliknite [ovdje](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="6dd6b-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="6dd6b-106">Bit će navedene dostupne mogućnosti prijave.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="6dd6b-107">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="6dd6b-107">For example:</span></span>

    ![Opcije prijave.](media/sign-in-options.png)

2. <span data-ttu-id="6dd6b-109">Kliknite ili dodirnite **Otisak prsta za Pozdrav u sustavu Windows**, a zatim **Postavi**.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="6dd6b-110">U prozoru za postavljanje značajke Windows Hello kliknite **Početak rada**.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="6dd6b-111">Senzor otiska prsta će se aktivirati, a vi ćete biti zatraženo da stavite prst na senzor:</span><span class="sxs-lookup"><span data-stu-id="6dd6b-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor otiska prsta.](media/fingerprint-sensor.png)

3. <span data-ttu-id="6dd6b-113">Slijedite upute koje će od vas zatražiti da više puta skenirate prst.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="6dd6b-114">Kada se to završi, moći ćete dodati druge prste koje biste mogli koristiti za prijavu.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="6dd6b-115">Sljedeći put kada se prijavite u Windows 10, imat ćete mogućnost korištenja otiska prsta da biste to učinili.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="6dd6b-116">**Otisak prsta za Pozdrav u sustavu Windows nije dostupan kao mogućnost prijave**</span><span class="sxs-lookup"><span data-stu-id="6dd6b-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="6dd6b-117">Ako se otisak prsta za Pozdrav u sustavu Windows ne prikazuje kao mogućnost u **mogućnostima prijave,** to znači da Windows nije svjestan čitača otisaka prstiju/skenera priključenog na PC ili da pravilo sustava sprječava njegovo korištenje (ako vašim PC-jem upravlja vaše radno mjesto).</span><span class="sxs-lookup"><span data-stu-id="6dd6b-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="6dd6b-118">Da biste otklonili poteškoće:</span><span class="sxs-lookup"><span data-stu-id="6dd6b-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="6dd6b-119">Odaberite gumb **Start** na programskoj traci i potražite **Upravitelj uređaja**.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="6dd6b-120">Klikom ili dodirom otvorite **Upravitelj uređaja**.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="6dd6b-121">U upravitelju uređaja proširite biometrijske uređaje klikom na njegov ševron.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrijski uređaji.](media/biometric-devices.png)

4. <span data-ttu-id="6dd6b-123">Skener otiska prsta trebao bi biti naveden kao biometrijski uređaj, kao što je Synaptics WBDI skener:</span><span class="sxs-lookup"><span data-stu-id="6dd6b-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrijski uređaji.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="6dd6b-125">Ako se skener otiska prsta ne prikaže, a skener je integriran u PC, posjetite web-mjesto proizvođača PC-ja.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="6dd6b-126">U odjeljku tehničke podrške za model PC-ja potražite upravljački program za Windows 10 za skener koji možete instalirati.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="6dd6b-127">Ako je skener odvojen od PC-ja (priključenog putem USB-a), posjetite web-mjesto proizvođača skenera da biste pronašli i instalirali upravljački program za upravljački program uređaja sustava Windows 10 za model skenera koji imate.</span><span class="sxs-lookup"><span data-stu-id="6dd6b-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
