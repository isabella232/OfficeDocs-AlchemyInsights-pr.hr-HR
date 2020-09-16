---
title: Otklanjanje poteškoća sa zvukom u sustavu Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750299"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="e2a9f-102">Otklanjanje poteškoća sa zvukom u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="e2a9f-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="e2a9f-103">**Pokretanje alata za otklanjanje poteškoća s zvukom**</span><span class="sxs-lookup"><span data-stu-id="e2a9f-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="e2a9f-104">Otvorite [Postavke otklanjanja poteškoća](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="e2a9f-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="e2a9f-105">Odaberite **reprodukcija zvuka**  >  **da biste pokrenuli alat za otklanjanje poteškoća**.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="e2a9f-106">**Postavljanje zadanog uređaja**</span><span class="sxs-lookup"><span data-stu-id="e2a9f-106">**Set the default device**</span></span>

<span data-ttu-id="e2a9f-107">Ako se povezujete s audiouređajem pomoću USB-a ili HDMI-ja, možda ćete morati postaviti taj uređaj kao zadani:</span><span class="sxs-lookup"><span data-stu-id="e2a9f-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="e2a9f-108">Otvorite **početni**  >  **zvuk**, a zatim na popisu rezultata odaberite **zvuk** ili **Promijeni zvukove sustava** .</span><span class="sxs-lookup"><span data-stu-id="e2a9f-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="e2a9f-109">Na kartici **Reprodukcija** odaberite uređaj, odaberite **Postavi zadano**, a zatim odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="e2a9f-110">**Provjera kabela, glasnoće, zvučnika i slušalica**</span><span class="sxs-lookup"><span data-stu-id="e2a9f-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="e2a9f-111">Provjerite veze zvučnika i slušalica za labavo kablove i provjerite jesu li povezani s ispravnom priključkom.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="e2a9f-112">Provjerite razine napajanja i glasnoće pa pokušajte isključiti sve kontrole glasnoće.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="e2a9f-113">Neki zvučnici i aplikacije imaju vlastite kontrole glasnoće; Možda ćete ih morati provjeriti sve da biste bili sigurni da su na pravim razinama.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="e2a9f-114">Pokušajte se povezati pomoću drugog USB priključka.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="e2a9f-115">**Imajte na umu**: zapamtite da zvučnici možda neće funkcionirati kada su slušalice priključene.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="e2a9f-116">**Provjera upravitelja uređaja**</span><span class="sxs-lookup"><span data-stu-id="e2a9f-116">**Check Device Manager**</span></span>

<span data-ttu-id="e2a9f-117">Da biste bili sigurni da su upravljački programi ažurirani, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="e2a9f-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="e2a9f-118">Odaberite **Start**, upišite **Upravitelj uređaja**, a zatim na popisu rezultata odaberite **Upravitelj uređaja** .</span><span class="sxs-lookup"><span data-stu-id="e2a9f-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="e2a9f-119">U odjeljku **Kontroleri za zvukove, videozapise i igre**Odaberite zvučnu karticu, otvorite je, odaberite karticu **upravljački** program, a zatim **Ažuriraj upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="e2a9f-120">**Napomena**: Ako Windows ne pronađe novi upravljački program, potražite ga na web-mjestu proizvođača uređaja i slijedite upute.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="e2a9f-121">**Ponovna instalacija upravljačkog programa**</span><span class="sxs-lookup"><span data-stu-id="e2a9f-121">**Reinstall the driver**</span></span>

<span data-ttu-id="e2a9f-122">Ako ne možete ažurirati putem upravitelja uređaja ili pronaći novi upravljački program na web-mjestu proizvođača, isprobajte sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="e2a9f-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="e2a9f-123">U upravitelju uređaja desnom tipkom miša kliknite (ili pritisnite i držite) upravljački program za audiouređaj, a zatim odaberite **Deinstaliraj**.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="e2a9f-124">Ponovno pokrenite uređaj i Windows će pokušati ponovno instalirati upravljački program.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="e2a9f-125">Ako ponovna instalacija upravljačkog programa ne funkcionira, pokušajte koristiti generički upravljački program za audiouređaj koji se isporučuje sa sustavom Windows.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="e2a9f-126">U upravitelju uređaja desnom tipkom miša kliknite (ili pritisnite i držite) upravljački program za audiouređaj > **ažurirati upravljački**program  >  **potražite na računalu upravljački softver**  >  **Dopusti mi izdvajanje s popisa upravljačkih programa uređaja na računalu**, odaberite **audiouređaj High definition**, odaberite **dalje**, a zatim slijedite upute da biste ga instalirali.</span><span class="sxs-lookup"><span data-stu-id="e2a9f-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
