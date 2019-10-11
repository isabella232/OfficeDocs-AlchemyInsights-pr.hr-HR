---
title: Zaglavljeni u izlaznim kutijama zbog velikih privitaka
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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441298"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="15caf-102">Ispravljanje poruka koje su zaglavljeno u izlazno polje</span><span class="sxs-lookup"><span data-stu-id="15caf-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="15caf-103">Preporučujemo da počnete pokretanjem scenarija ["Imam problema s slanjem, primanjem ili pronalaženjem poruka e-pošte"](https://aka.ms/SaRA-OutlookSendReceive) iz alata [Microsoftova pomoćnika za podršku i oporavak](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="15caf-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="15caf-104">Kada se poruka zaglavi u izlaznim sanducima, najvjerojatniji uzroci su:</span><span class="sxs-lookup"><span data-stu-id="15caf-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="15caf-105">Veliki privici.</span><span class="sxs-lookup"><span data-stu-id="15caf-105">Large attachments.</span></span>
- <span data-ttu-id="15caf-106">**Pošalji odmah kada je povezana** opcija nije omogućena.</span><span class="sxs-lookup"><span data-stu-id="15caf-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="15caf-107">Da biste uklonili velike privitke:</span><span class="sxs-lookup"><span data-stu-id="15caf-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="15caf-108">U programu Outlook odaberite **slanje/primanje** > **radi izvanmrežno**.</span><span class="sxs-lookup"><span data-stu-id="15caf-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="15caf-109">U navigacijskom oknu odaberite **izlazno polje**.</span><span class="sxs-lookup"><span data-stu-id="15caf-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="15caf-110">Odavde možete:</span><span class="sxs-lookup"><span data-stu-id="15caf-110">From here, you can:</span></span> 
    - <span data-ttu-id="15caf-111">Izbrišite poruku (odaberite je, a zatim odaberite **Izbriši**).</span><span class="sxs-lookup"><span data-stu-id="15caf-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="15caf-112">Povucite poruku u mapu Skice, dvokliknite da biste je otvorili i uklonite privitak, odaberite ga, a zatim odaberite **Izbriši**).</span><span class="sxs-lookup"><span data-stu-id="15caf-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="15caf-113">Ako primite pogrešku koja kaže da Outlook pokušava prenijeti poruku, zatvorite Outlook.</span><span class="sxs-lookup"><span data-stu-id="15caf-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="15caf-114">Možda će trebati nekoliko trenutaka da izađete.</span><span class="sxs-lookup"><span data-stu-id="15caf-114">It may take a few moments to exit.</span></span> <span data-ttu-id="15caf-115">Ako se Outlook ne zatvara, pritisnite CTRL + ALT + DELETE i odaberite **Pokreni upravitelj zadataka**.</span><span class="sxs-lookup"><span data-stu-id="15caf-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="15caf-116">U upravitelju zadataka odaberite karticu **procesi** , pomaknite se prema dolje u Outlook. exe i odaberite **završetak procesa**.</span><span class="sxs-lookup"><span data-stu-id="15caf-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="15caf-117">Nakon što se Outlook zatvori, ponovno ga pokrenite i ponovite korake 2 i 3.</span><span class="sxs-lookup"><span data-stu-id="15caf-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="15caf-118">Nakon što uklonite privitak, pritisnite **Pošalji/primi** > **Izvanmrežni rad** da biste nastavili raditi na mreži.</span><span class="sxs-lookup"><span data-stu-id="15caf-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="15caf-119">Poruke se također zaglave u izlaznu kutiju kada kliknete **Pošalji**, ali niste povezani.</span><span class="sxs-lookup"><span data-stu-id="15caf-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="15caf-120">Kliknite **Pošalji/primi** i pogledajte gumb **Izvanmrežni rad** .</span><span class="sxs-lookup"><span data-stu-id="15caf-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="15caf-121">Ako je plavo, isključen si.</span><span class="sxs-lookup"><span data-stu-id="15caf-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="15caf-122">Odaberite ga za povezivanje (gumb postaje bijel) i kliknite **Pošalji sve**.</span><span class="sxs-lookup"><span data-stu-id="15caf-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="15caf-123">Da biste omogućili **Slanje odmah kada ste povezani**:</span><span class="sxs-lookup"><span data-stu-id="15caf-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="15caf-124">Odaberite \*\*\*\* > \*\*\*\* mogućnosti >  datoteke**napredne**.</span><span class="sxs-lookup"><span data-stu-id="15caf-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="15caf-125">U sekciji **Slanje i primanje** odaberite **Pošalji odmah kada je spojen**, a zatim odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="15caf-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="15caf-126">Za sve detalje pogledajte:</span><span class="sxs-lookup"><span data-stu-id="15caf-126">For full details see:</span></span>
- [<span data-ttu-id="15caf-127">Videozapis: slanje ili brisanje zaglavljeno e-pošte</span><span class="sxs-lookup"><span data-stu-id="15caf-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="15caf-128">E-pošta ostaje u mapi Outbox dok ručno ne pokrenete operaciju slanja/primanja u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="15caf-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
