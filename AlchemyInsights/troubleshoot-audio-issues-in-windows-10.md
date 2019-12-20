---
title: Rješavanje problema s zvukom u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796011"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="67fd5-102">Rješavanje problema s zvukom u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="67fd5-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="67fd5-103">**Pokretanje alata za otklanjanje poteškoća s zvukom**</span><span class="sxs-lookup"><span data-stu-id="67fd5-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="67fd5-104">Alat za otklanjanje poteškoća s zvukom možda može automatski ispraviti probleme s zvukom:</span><span class="sxs-lookup"><span data-stu-id="67fd5-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="67fd5-105">Odaberite **Start**, upišite **Otklanjanje poteškoća**, a zatim odaberite **Otklanjanje poteškoća** s popisa rezultata.</span><span class="sxs-lookup"><span data-stu-id="67fd5-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="67fd5-106">Odaberite **Reprodukcija audiozapisa** > **Pokreni alat za otklanjanje poteškoća**.</span><span class="sxs-lookup"><span data-stu-id="67fd5-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="67fd5-107">**Provjerite kabele, glasnoću, zvučnike i slušalice**</span><span class="sxs-lookup"><span data-stu-id="67fd5-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="67fd5-108">Provjerite ima li zvučnik i slušalice veze za labave kabele i provjerite jesu li spojeni na ispravan priključak.</span><span class="sxs-lookup"><span data-stu-id="67fd5-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="67fd5-109">Provjerite razinu napajanja i glasnoće i pokušajte pretvoriti sve kontrole glasnoće.</span><span class="sxs-lookup"><span data-stu-id="67fd5-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="67fd5-110">Neki zvučnici i aplikacije imaju svoje kontrole glasnoće, i možda ćete morati provjeriti sve kako bi bili sigurni da su na pravom nivou.</span><span class="sxs-lookup"><span data-stu-id="67fd5-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="67fd5-111">Pokušajte povezati pomoću drugog USB priključka.</span><span class="sxs-lookup"><span data-stu-id="67fd5-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="67fd5-112">**Napomena:** Sjetite se da zvučnici možda neće raditi kada su priključene slušalice.</span><span class="sxs-lookup"><span data-stu-id="67fd5-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="67fd5-113">**Provjeri upravitelja uređaja**</span><span class="sxs-lookup"><span data-stu-id="67fd5-113">**Check Device Manager**</span></span>

<span data-ttu-id="67fd5-114">Da biste bili sigurni da su upravljački programi ažurirani:</span><span class="sxs-lookup"><span data-stu-id="67fd5-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="67fd5-115">Odaberite **Start**, upišite **Upravitelj uređaja**, a zatim odaberite **Upravitelj uređaja** s popisa rezultata.</span><span class="sxs-lookup"><span data-stu-id="67fd5-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="67fd5-116">U odjeljku **Kontroleri zvuka, videozapisa i igre**Odaberite zvučnu karticu, otvorite je, odaberite karticu **upravljački program** i odaberite **Ažuriraj upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="67fd5-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="67fd5-117">**Napomena:** Ako Windows ne pronađe novi upravljački program, potražite ga na web-mjestu proizvođača uređaja i slijedite njihove upute.</span><span class="sxs-lookup"><span data-stu-id="67fd5-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="67fd5-118">**Ponovna instalacija upravljačkog programa**</span><span class="sxs-lookup"><span data-stu-id="67fd5-118">**Reinstall the driver**</span></span>

<span data-ttu-id="67fd5-119">Ako ne možete ažurirati putem upravitelja uređaja ili pronaći novi upravljački program na web-mjestu proizvođača, pokušajte ove korake:</span><span class="sxs-lookup"><span data-stu-id="67fd5-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="67fd5-120">U upravitelju uređaja desnom tipkom miša kliknite (ili pritisnite i držite) upravljački program za audio i odaberite **Deinstaliraj**.</span><span class="sxs-lookup"><span data-stu-id="67fd5-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="67fd5-121">Ponovno pokrenite uređaj i Windows će pokušati ponovno instalirati upravljački program.</span><span class="sxs-lookup"><span data-stu-id="67fd5-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="67fd5-122">Ako ponovna instalacija upravljačkog programa ne radi, pokušajte koristiti generički upravljački program za audiozapise koji dolazi sa sustavom Windows.</span><span class="sxs-lookup"><span data-stu-id="67fd5-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="67fd5-123">U upravitelju uređaja desnom tipkom miša kliknite (ili pritisnite i držite) vaš upravljački program za audio > **Update Driver softver** > **Pregledajte moje računalo za upravljački** > program**Dopustite mi da izaberem s popisa upravljačkih programa uređaja na računalu**, odaberite **audiouređaj visoke razlučivosti**, odaberite **dalje**i slijedite upute da biste ga instalirali.</span><span class="sxs-lookup"><span data-stu-id="67fd5-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="67fd5-124">**Postavljanje zadanog uređaja**</span><span class="sxs-lookup"><span data-stu-id="67fd5-124">**Set the default device**</span></span>

<span data-ttu-id="67fd5-125">Ako se priključujete na audio uređaj pomoću USB ili HDMI, možda ćete morati postaviti taj uređaj kao zadani:</span><span class="sxs-lookup"><span data-stu-id="67fd5-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="67fd5-126">Odaberite **Start**, upišite **zvuk**, a zatim odaberite **zvuk** ili **Promjena zvukova sustava** s popisa rezultata.</span><span class="sxs-lookup"><span data-stu-id="67fd5-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="67fd5-127">Na kartici **Reprodukcija** odaberite uređaj, odaberite **Postavi zadano**, a zatim odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="67fd5-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

