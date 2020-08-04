---
title: Korištenje programa TeamViewer za daljinsko administriranje intune uređaja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554774"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="145c8-102">Korištenje programa TeamViewer za daljinsko administriranje intune uređaja</span><span class="sxs-lookup"><span data-stu-id="145c8-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="145c8-103">Uređaji kojima upravlja Intune mogu se daljinski upravljati pomoću [programa TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="145c8-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="145c8-104">Da biste upravljali intune pomoću programa TeamViewer, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="145c8-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="145c8-105">Započnite dohvaćanjem vjerodajnica od programa TeamViewer da biste postavili TeamViewer Connector na intune.</span><span class="sxs-lookup"><span data-stu-id="145c8-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="145c8-106">To administratoru omogućuje unos vjerodajnica u korisničko ime programa TeamViewer Connector u odjeljku Uređaji, jednokratna operacija za uspostavljanje veze između servisa Intune i usluge TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="145c8-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="145c8-107">**1. dio: pokretanje sesije pomoću udaljenog uređaja**</span><span class="sxs-lookup"><span data-stu-id="145c8-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="145c8-108">U odjeljku **Svi uređaji**odaberite uređaj s kojim želite pokrenuti udaljenu sesiju.</span><span class="sxs-lookup"><span data-stu-id="145c8-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="145c8-109">Od **... Dodatne**postavke odaberite **Nova sesija daljinske pomoći**.</span><span class="sxs-lookup"><span data-stu-id="145c8-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="145c8-110">Odaberite **Da** da biste potvrdili da želite uspostaviti udaljenu sesiju.</span><span class="sxs-lookup"><span data-stu-id="145c8-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="145c8-111">Nakon što servis TeamViewer potvrdi zahtjev "Pokretanje nove udaljene sesije", vidjet ćete mogućnost **pokretanja daljinske pomoći** pod detaljima okna Pregled (ili Essentials) za uređaj.</span><span class="sxs-lookup"><span data-stu-id="145c8-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="145c8-112">Odaberite **Vidi više** da biste proširili okno i prikazali status daljinske pomoći.</span><span class="sxs-lookup"><span data-stu-id="145c8-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="145c8-113">Odaberite **Pokreni udaljenu sesiju** da biste pokrenuli sesiju na strani administratora.</span><span class="sxs-lookup"><span data-stu-id="145c8-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="145c8-114">Odaberite preuzimanje binarnog programa TeamViewer (Windows), a zatim odaberite **Pokreni**.</span><span class="sxs-lookup"><span data-stu-id="145c8-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="145c8-115">**Napomena:** Možete zanemariti bilo koju stranicu web-preglednika otvorenu na web-mjestu Programa TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="145c8-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="145c8-116">Potvrdite zahtjev za aplikaciju TeamViewer da biste unijeli promjene na uređaju (samo Windows).</span><span class="sxs-lookup"><span data-stu-id="145c8-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="145c8-117">Pokreće se aplikacija TeamViewer i uključuje kôd sesije za provjeru autentičnosti veze s udaljenim uređajem.</span><span class="sxs-lookup"><span data-stu-id="145c8-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="145c8-118">**Dio 2: Na uređaju koji se cilja za udaljenu sesiju**</span><span class="sxs-lookup"><span data-stu-id="145c8-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="145c8-119">Otvorite portal tvrtke Intune.</span><span class="sxs-lookup"><span data-stu-id="145c8-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="145c8-120">Potražite zastavicu obavijesti: "Vaš IT administrator traži kontrolu nad ovim uređajem za sesiju daljinske pomoći" i odaberite obavijest.</span><span class="sxs-lookup"><span data-stu-id="145c8-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="145c8-121">Odaberite preuzimanje aplikacije TeamViewer ili potvrdite preuzimanje aplikacije TeamViewer iz trgovine aplikacija i odaberite **Pokreni**.</span><span class="sxs-lookup"><span data-stu-id="145c8-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="145c8-122">**Napomena:** Možete zanemariti bilo koju stranicu web-preglednika otvorenu na web-mjestu Programa TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="145c8-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="145c8-123">Potvrdite zahtjev za aplikaciju TeamViewer da biste unijeli promjene na uređaju (samo Windows).</span><span class="sxs-lookup"><span data-stu-id="145c8-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="145c8-124">Pokreće se aplikacija TeamViewer i uključuje kôd sesije za provjeru autentičnosti veze s udaljenim uređajem.</span><span class="sxs-lookup"><span data-stu-id="145c8-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="145c8-125">Skočni prozor pita želite li dopustiti pokretanje sesije.</span><span class="sxs-lookup"><span data-stu-id="145c8-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="145c8-126">**Napomena:** Šifre sesija koje generira usluga TeamViewer jednokratno su upotreba.</span><span class="sxs-lookup"><span data-stu-id="145c8-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="145c8-127">Ako izgubite vezu, morate:</span><span class="sxs-lookup"><span data-stu-id="145c8-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="145c8-128">Zatvorite instancu aplikacije TeamViewer na udaljenom uređaju i na upravljačkoj radnoj stanici.</span><span class="sxs-lookup"><span data-stu-id="145c8-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="145c8-129">Zatvorite portal tvrtke na udaljenom uređaju.</span><span class="sxs-lookup"><span data-stu-id="145c8-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="145c8-130">Pokrenite novu "Novu sesiju daljinske pomoći" s portala za administratore.</span><span class="sxs-lookup"><span data-stu-id="145c8-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="145c8-131">Ponovno otvorite portal tvrtke na udaljenom uređaju da biste primili novu obavijest.</span><span class="sxs-lookup"><span data-stu-id="145c8-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="145c8-132">Preuzmite i otvorite aplikaciju TeamViewer na udaljenom uređaju i na administratorsku radnu stanicu, kao i prije.</span><span class="sxs-lookup"><span data-stu-id="145c8-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>