---
title: Zaglavi u izlaznoj pošti zbog velikih privitaka
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241244"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="8812e-102">Ispravljanje poruka koje su zaglavljene u izlaznoj pošti</span><span class="sxs-lookup"><span data-stu-id="8812e-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="8812e-103">Preporučujemo da pokrenete scenarij ["Imam problema sa slanjem, primanjem ili pronalaženjem poruka e-pošte"](https://aka.ms/SaRA-OutlookSendReceive) iz alata [Microsoftovpomoćnik za podršku i oporavak.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="8812e-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="8812e-104">Kada se poruka zaglavi u izlaznoj pošti, najvjerojatniji uzrok je veliki privitak ili opcija "Pošalji odmah kada je povezan" nije omogućena.</span><span class="sxs-lookup"><span data-stu-id="8812e-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="8812e-105">**Uklanjanje velikog privitka**</span><span class="sxs-lookup"><span data-stu-id="8812e-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="8812e-106">U programu Outlook odaberite **Slanje / primanje** > **izvanmrežnog rada**.</span><span class="sxs-lookup"><span data-stu-id="8812e-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="8812e-107">U navigacijskom oknu odaberite **Izlazna pošta**.</span><span class="sxs-lookup"><span data-stu-id="8812e-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="8812e-108">Odavde možete:</span><span class="sxs-lookup"><span data-stu-id="8812e-108">From here, you can:</span></span> 
    - <span data-ttu-id="8812e-109">Izbrišite poruku (odaberite je, a zatim odaberite **Izbriši**).</span><span class="sxs-lookup"><span data-stu-id="8812e-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="8812e-110">Povucite poruku u mapu Skice, dvokliknite da biste je otvorili i uklonite privitak, odaberite je, a zatim odaberite **Izbriši**).</span><span class="sxs-lookup"><span data-stu-id="8812e-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="8812e-111">Ako primite poruku koja kaže da Outlook pokušava prenijeti poruku, zatvorite Outlook.</span><span class="sxs-lookup"><span data-stu-id="8812e-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="8812e-112">Možda će trebati nekoliko trenutaka da izađete.</span><span class="sxs-lookup"><span data-stu-id="8812e-112">It may take a few moments to exit.</span></span> <span data-ttu-id="8812e-113">Ako se Outlook ne zatvori, pritisnite Ctrl+Alt+Delete i odaberite **Pokreni upravitelj zadataka**.</span><span class="sxs-lookup"><span data-stu-id="8812e-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="8812e-114">U upravitelju zadataka odaberite karticu **Procesi,** pomaknite se prema dolje do datoteke outlook.exe i odaberite **Završi proces**.</span><span class="sxs-lookup"><span data-stu-id="8812e-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="8812e-115">Nakon zatvaranja programa Outlook ponovno ga pokrenite i ponovite korake 2 i 3.</span><span class="sxs-lookup"><span data-stu-id="8812e-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="8812e-116">Nakon što uklonite privitak, kliknite **Pošalji / primi** > **izvanmrežni rad** da biste nastavili raditi na mreži.</span><span class="sxs-lookup"><span data-stu-id="8812e-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="8812e-117">Poruke se zaglave i u izlaznoj pošti kada kliknete **Pošalji**, ali niste povezani.</span><span class="sxs-lookup"><span data-stu-id="8812e-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="8812e-118">Kliknite **Slanje/primanje** i pogledajte gumb **Izvanmrežni rad.**</span><span class="sxs-lookup"><span data-stu-id="8812e-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="8812e-119">Ako je plava, isključen si.</span><span class="sxs-lookup"><span data-stu-id="8812e-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="8812e-120">Kliknite ga da biste se povezali (gumb pobijeli) i kliknite **Pošalji sve**.</span><span class="sxs-lookup"><span data-stu-id="8812e-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="8812e-121">**Omogući slanje odmah nakon povezivanja**</span><span class="sxs-lookup"><span data-stu-id="8812e-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="8812e-122">Na kartici Datoteka kliknite **Mogućnosti**.</span><span class="sxs-lookup"><span data-stu-id="8812e-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="8812e-123">U dijaloškom okviru Mogućnosti programa Outlook kliknite **Dodatno**.</span><span class="sxs-lookup"><span data-stu-id="8812e-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="8812e-124">U odjeljku Slanje i primanje kliknite da biste omogućili **slanje odmah nakon povezivanja**.</span><span class="sxs-lookup"><span data-stu-id="8812e-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="8812e-125">Kliknite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="8812e-125">Click **OK**.</span></span>
 
<span data-ttu-id="8812e-126">Za sve pojedinosti pogledajte:</span><span class="sxs-lookup"><span data-stu-id="8812e-126">For full details, see:</span></span>
- [<span data-ttu-id="8812e-127">Videozapis: Slanje ili brisanje zaglavljene e-pošte</span><span class="sxs-lookup"><span data-stu-id="8812e-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="8812e-128">E-pošta ostaje u mapi Izlazna pošta dok ručno ne pokrenete operaciju slanja / primanja u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="8812e-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
