---
title: Web-dijelovi servisa Yammer u sustavu SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: d8b4043bb2889429a18c477505e7eca662943051
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664342"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="439b2-102">Web-dijelovi servisa Yammer u sustavu SharePoint</span><span class="sxs-lookup"><span data-stu-id="439b2-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="439b2-103">Razgovori servisa Yammer i web-dijelovi servisa Yammer poboljšavaju suradnju na modernim i klasičnim stranicama sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="439b2-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="439b2-104">Dodatne informacije potražite u članku [razgovori sa servisom Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  i  [istaknute značajke servisa Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span><span class="sxs-lookup"><span data-stu-id="439b2-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="439b2-105">Moderni web-dio razgovora servisa Yammer ažuriran je na novo iskustvo servisa Yammer i dostupan je za ciljano izdanje stanara.</span><span class="sxs-lookup"><span data-stu-id="439b2-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="439b2-106">Pokrenuta je primjena GA.</span><span class="sxs-lookup"><span data-stu-id="439b2-106">GA rollout has started.</span></span> <span data-ttu-id="439b2-107">Nove značajke uključuju mogućnost pokretanja razgovora s bilo kojim objavom (pitanja, ankete, pohvala) i označavanje najboljih odgovora izravno iz sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="439b2-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="439b2-108">Dodatne informacije potražite u članku [novi uvjeti za korisnike servisa Yammer i najčešća pitanja](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span><span class="sxs-lookup"><span data-stu-id="439b2-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="439b2-109">Da biste razumjeli koji su web-dio i konfiguracija pravi za vas, pročitajte članak [korištenje web-dijela servisa Yammer u sustavu SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span><span class="sxs-lookup"><span data-stu-id="439b2-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="439b2-110">**Korištenje web-dijelova sa sustavom SharePoint Server**</span><span class="sxs-lookup"><span data-stu-id="439b2-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="439b2-111">Web-dijelovi mogu se koristiti u modernim i klasičnim stranicama unutar lokalnih okruženja.</span><span class="sxs-lookup"><span data-stu-id="439b2-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="439b2-112">Dodatne informacije o modernim stranicama potražite u članku [Dodavanje sažetka sadržaja servisa Yammer na modernu stranicu u sustavu SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span><span class="sxs-lookup"><span data-stu-id="439b2-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="439b2-113">Dodatne informacije o klasičnim stranicama potražite u članku [Dodavanje sažetka sadržaja servisa Yammer na klasičnu stranicu u sustavu SharePoint Servers 2013, 2016 i 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span><span class="sxs-lookup"><span data-stu-id="439b2-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="439b2-114">**Ugradnja servisa Yammer**</span><span class="sxs-lookup"><span data-stu-id="439b2-114">**Yammer Embed**</span></span>  

<span data-ttu-id="439b2-115">Koristite alat za konfiguraciju ugrađivanja da biste testirali korištenje ugrađivanja.</span><span class="sxs-lookup"><span data-stu-id="439b2-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="439b2-116">Buduće ažuriranje za ugrađivanje omogućit će novo iskustvo servisa Yammer.</span><span class="sxs-lookup"><span data-stu-id="439b2-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="439b2-117">Dodatne informacije potražite u članku [alat za konfiguraciju ugrađivanja servisa Yammer](https://aka.ms/YammerEmbedConfigureTool).</span><span class="sxs-lookup"><span data-stu-id="439b2-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="439b2-118">Da biste bolje razumjeli komponentu ugrađivanja servisa Yammer, pročitajte članak [ugradnja sažetka sadržaja](https://aka.ms/YammerDevDocs).</span><span class="sxs-lookup"><span data-stu-id="439b2-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="439b2-119">**Poznati problemi i ograničenja**</span><span class="sxs-lookup"><span data-stu-id="439b2-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="439b2-120">Grupe ID-ovi nisu dostupni iz novih URL-ova servisa Yammer koje su se promijenile.</span><span class="sxs-lookup"><span data-stu-id="439b2-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="439b2-121">Vratite se u klasični način da biste nabavili ID-ove ili druge ID-ove iz URL-ova.</span><span class="sxs-lookup"><span data-stu-id="439b2-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="439b2-122">Custom (Vanity) domene nisu podržane.</span><span class="sxs-lookup"><span data-stu-id="439b2-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="439b2-123">Ugradnja servisa Yammer nije optimizirana za mobilne uređaje.</span><span class="sxs-lookup"><span data-stu-id="439b2-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="439b2-124">Koristite moderne stranice s web-dijelom razgovora servisa Yammer za najbolje iskustvo.</span><span class="sxs-lookup"><span data-stu-id="439b2-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="439b2-125">Prilagođene teme mogu utjecati na izgled i upotrebljivost web-dijela razgovora servisa Yammer.</span><span class="sxs-lookup"><span data-stu-id="439b2-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="439b2-126">Otvaranje slučaja podrške radi izvješća o problemima.</span><span class="sxs-lookup"><span data-stu-id="439b2-126">Open a support case to report issues.</span></span>