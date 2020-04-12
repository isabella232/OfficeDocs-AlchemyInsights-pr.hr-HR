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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232622"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="e6a78-102">Ispravljanje poruka koje su zaglavljene u izlaznoj pošti</span><span class="sxs-lookup"><span data-stu-id="e6a78-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="e6a78-103">Preporučujemo da pokrenete scenarij ["Imam problema sa slanjem, primanjem ili pronalaženjem poruka e-pošte"](https://aka.ms/SaRA-OutlookSendReceive) iz alata [Microsoftovpomoćnik za podršku i oporavak](https://diagnostics.office.com/#/) na zahvaćenom računalu.</span><span class="sxs-lookup"><span data-stu-id="e6a78-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="e6a78-104">Kada se poruka zaglavi u izlaznoj pošti, najvjerojatniji uzrok je veliki privitak ili opcija "Pošalji odmah kada je povezan" nije omogućena.</span><span class="sxs-lookup"><span data-stu-id="e6a78-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="e6a78-105">**Uklanjanje velikog privitka**</span><span class="sxs-lookup"><span data-stu-id="e6a78-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="e6a78-106">Kliknite **Slanje / primanje** > **posla izvanmrežno**.</span><span class="sxs-lookup"><span data-stu-id="e6a78-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="e6a78-107">U navigacijskom oknu kliknite **Izlazna pošta**.</span><span class="sxs-lookup"><span data-stu-id="e6a78-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="e6a78-108">Odavde možete:</span><span class="sxs-lookup"><span data-stu-id="e6a78-108">From here, you can:</span></span> 
    - <span data-ttu-id="e6a78-109">Izbrišite poruku.</span><span class="sxs-lookup"><span data-stu-id="e6a78-109">Delete the message.</span></span> <span data-ttu-id="e6a78-110">Samo ga odaberite i kliknite **Izbriši**.</span><span class="sxs-lookup"><span data-stu-id="e6a78-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="e6a78-111">Povucite poruku u **mapu skica,** dvokliknite da biste otvorili poruku i izbrišite privitak (kliknite ga i kliknite **Izbriši).**</span><span class="sxs-lookup"><span data-stu-id="e6a78-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="e6a78-112">Ako vam pogreška kaže da Outlook pokušava prenijeti poruku, zatvorite Outlook.</span><span class="sxs-lookup"><span data-stu-id="e6a78-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="e6a78-113">Možda će trebati nekoliko trenutaka da izađete.</span><span class="sxs-lookup"><span data-stu-id="e6a78-113">It may take a few moments to exit.</span></span> <span data-ttu-id="e6a78-114">Ako se Outlook ne zatvori, pritisnite **Ctrl+Alt+Delete,** a zatim kliknite **Pokreni upravitelj zadataka**.</span><span class="sxs-lookup"><span data-stu-id="e6a78-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="e6a78-115">U upravitelju zadataka odaberite karticu **Procesi,** pomaknite se prema dolje do datoteke outlook.exe, a zatim kliknite **Završi proces**.</span><span class="sxs-lookup"><span data-stu-id="e6a78-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="e6a78-116">Nakon zatvaranja programa Outlook ponovno pokrenite Outlook i ponovite korake 2-3.</span><span class="sxs-lookup"><span data-stu-id="e6a78-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="e6a78-117">Nakon što uklonite privitak, kliknite **Pošalji / primi** > **posao izvanmrežno** da biste poništili odabir gumba i nastavili raditi na mreži.</span><span class="sxs-lookup"><span data-stu-id="e6a78-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="e6a78-118">Poruke se zaglave i u izlaznoj pošti kada kliknete **Pošalji**, ali niste povezani.</span><span class="sxs-lookup"><span data-stu-id="e6a78-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="e6a78-119">Kliknite **Slanje/primanje** i pogledajte gumb **Izvanmrežni rad.**</span><span class="sxs-lookup"><span data-stu-id="e6a78-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="e6a78-120">Ako je plava, isključen si.</span><span class="sxs-lookup"><span data-stu-id="e6a78-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="e6a78-121">Kliknite ga da biste se povezali (gumb pobijeli) i kliknite **Pošalji sve**.</span><span class="sxs-lookup"><span data-stu-id="e6a78-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="e6a78-122">**Omogući slanje odmah nakon povezivanja**</span><span class="sxs-lookup"><span data-stu-id="e6a78-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="e6a78-123">Na kartici Datoteka kliknite **Mogućnosti**.</span><span class="sxs-lookup"><span data-stu-id="e6a78-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="e6a78-124">U dijaloškom okviru Mogućnosti programa Outlook kliknite **Dodatno**.</span><span class="sxs-lookup"><span data-stu-id="e6a78-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="e6a78-125">U odjeljku Slanje i primanje kliknite da biste omogućili **slanje odmah nakon povezivanja**.</span><span class="sxs-lookup"><span data-stu-id="e6a78-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="e6a78-126">Kliknite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="e6a78-126">Click **OK**.</span></span>
 
<span data-ttu-id="e6a78-127">Za sve pojedinosti pogledajte:</span><span class="sxs-lookup"><span data-stu-id="e6a78-127">For full details, see:</span></span>
- [<span data-ttu-id="e6a78-128">Videozapis: Slanje ili brisanje zaglavljene e-pošte</span><span class="sxs-lookup"><span data-stu-id="e6a78-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="e6a78-129">E-pošta ostaje u mapi Izlazna pošta dok ručno ne pokrenete operaciju slanja / primanja u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="e6a78-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
