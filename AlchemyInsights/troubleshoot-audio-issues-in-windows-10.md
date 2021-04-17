---
title: Otklanjanje poteškoća sa zvukom u sustavu Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833283"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="90dd5-102">Otklanjanje poteškoća sa zvukom u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="90dd5-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="90dd5-103">**Pokretanje alata za otklanjanje poteškoća sa zvukom**</span><span class="sxs-lookup"><span data-stu-id="90dd5-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="90dd5-104">Otvorite postavke [otklanjanja poteškoća](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="90dd5-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="90dd5-105">Odaberite **Reprodukcija**  >  **zvuka Pokrenite alat za otklanjanje poteškoća**.</span><span class="sxs-lookup"><span data-stu-id="90dd5-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="90dd5-106">**Postavljanje zadanog uređaja**</span><span class="sxs-lookup"><span data-stu-id="90dd5-106">**Set the default device**</span></span>

<span data-ttu-id="90dd5-107">Ako se s audiouređaj povezujete putem USB-a ili HDMI-a, možda ćete taj uređaj morati postaviti kao zadani:</span><span class="sxs-lookup"><span data-stu-id="90dd5-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="90dd5-108">Otvorite **Izbornik** Zvuk , a zatim na popisu rezultata  >   **odaberite Zvuk** ili Promijeni sistemske zvukove. </span><span class="sxs-lookup"><span data-stu-id="90dd5-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="90dd5-109">Na kartici **Reprodukcija** odaberite uređaj, odaberite **Postavi zadano**, a zatim U **redu**.</span><span class="sxs-lookup"><span data-stu-id="90dd5-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="90dd5-110">**Provjera kabela, glasnoće, zvučnika i slušalica**</span><span class="sxs-lookup"><span data-stu-id="90dd5-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="90dd5-111">Provjerite jesu li kabeli za zvučnike i slušalice labavi te jesu li povezani s pravilnom utičnicom.</span><span class="sxs-lookup"><span data-stu-id="90dd5-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="90dd5-112">Provjerite razinu napajanja i glasnoće i pokušajte pojašnjati sve kontrole glasnoće.</span><span class="sxs-lookup"><span data-stu-id="90dd5-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="90dd5-113">Neki zvučnici i aplikacije imaju vlastite kontrole glasnoće; možda ćete ih morati sve provjeriti da biste bili sigurni da su na pravom nivou.</span><span class="sxs-lookup"><span data-stu-id="90dd5-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="90dd5-114">Pokušajte se povezati pomoću drugog USB priključka.</span><span class="sxs-lookup"><span data-stu-id="90dd5-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="90dd5-115">**Napomena:** Imajte na umu da zvučnici možda neće funkcionirati kada su priključene slušalice.</span><span class="sxs-lookup"><span data-stu-id="90dd5-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="90dd5-116">**Provjera upravitelja uređaja**</span><span class="sxs-lookup"><span data-stu-id="90dd5-116">**Check Device Manager**</span></span>

<span data-ttu-id="90dd5-117">Da biste bili sigurni da su upravljački programi aute:</span><span class="sxs-lookup"><span data-stu-id="90dd5-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="90dd5-118">Odaberite **Start**, **upišite Upravitelj** uređaja , a zatim **na** popisu rezultata odaberite Upravitelj uređaja.</span><span class="sxs-lookup"><span data-stu-id="90dd5-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="90dd5-119">U **odjeljku Kontroleri za zvuk, videozapise** i igre odaberite zvučnu karticu, otvorite je, odaberite **karticu Upravljački** program pa odaberite Ažuriraj upravljački **program**.</span><span class="sxs-lookup"><span data-stu-id="90dd5-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="90dd5-120">**Napomena:** ako Windows ne pronađe novi upravljački program, potražite ga na web-mjestu proizvođača uređaja i slijedite njihove upute.</span><span class="sxs-lookup"><span data-stu-id="90dd5-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="90dd5-121">**Ponovna instalacija upravljačkog programa**</span><span class="sxs-lookup"><span data-stu-id="90dd5-121">**Reinstall the driver**</span></span>

<span data-ttu-id="90dd5-122">Ako ne možete ažurirati putem upravitelja uređaja ili pronaći novi upravljački program na web-mjestu proizvođača, isprobajte sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="90dd5-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="90dd5-123">U upravitelju uređaja desnom tipkom miša kliknite (ili pritisnite i držite) upravljački program za audiodatoteka, a zatim odaberite **Deinstaliraj**.</span><span class="sxs-lookup"><span data-stu-id="90dd5-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="90dd5-124">Ponovno pokrenite uređaj i Windows će pokušati ponovno instalirati upravljački program.</span><span class="sxs-lookup"><span data-stu-id="90dd5-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="90dd5-125">Ako ponovna instalacija upravljačkog programa ne funkcionira, pokušajte koristiti generički upravljački program za zvuk koji se isporučuje sa sustavom Windows.</span><span class="sxs-lookup"><span data-stu-id="90dd5-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="90dd5-126">U upravitelju uređaja desnom tipkom miša kliknite (ili pritisnite i držite) upravljački program za audiodatoteku > Ažuriraj upravljački program Pregledajte moje računalo za upravljački program Dopustite mi da s popisa upravljačkih programa uređaja na računalu odaberete Audiouređaj visoke razlučivosti , odaberite Dalje , a zatim slijedite upute  >    >  da biste ga instalirali. </span><span class="sxs-lookup"><span data-stu-id="90dd5-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
