---
title: Web-dijelovi servisa Yammer u sustavu SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: 6868d7cdbbcc7d73e7e65fa0b0c954b4cba619ff
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197795"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="b11da-102">Web-dijelovi servisa Yammer u sustavu SharePoint</span><span class="sxs-lookup"><span data-stu-id="b11da-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="b11da-103">Web-dijelovi značajke Yammer i Yammer ističe poboljšavaju suradnju na modernim i klasičnim stranicama sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b11da-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="b11da-104">Dodatne informacije potražite u [odjeljku Razgovori za Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations) i [Isticanja servisa Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span><span class="sxs-lookup"><span data-stu-id="b11da-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="b11da-105">Moderni web-dio razgovora servisa Yammer ažurira se na novi doživljaj servisa Yammer i dostupan je za ciljano izdanje stanara.</span><span class="sxs-lookup"><span data-stu-id="b11da-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="b11da-106">GA uvođenje je počelo.</span><span class="sxs-lookup"><span data-stu-id="b11da-106">GA rollout has started.</span></span> <span data-ttu-id="b11da-107">Nove značajke uključuju mogućnost pokretanja razgovora s bilo kojim postom (pitanja, ankete, pohvale) i označavanje najboljih odgovora izravno iz sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b11da-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="b11da-108">Dodatne informacije potražite [u odjeljku Novi uvjeti i najčešća pitanja o klijentima servisa Yammer](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span><span class="sxs-lookup"><span data-stu-id="b11da-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="b11da-109">Da biste razumjeli koji su web-dio i konfiguracija pravi za vas, pročitajte odjeljak [Korištenje web-dijela servisa Yammer u sustavu SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span><span class="sxs-lookup"><span data-stu-id="b11da-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="b11da-110">**Korištenje web-dijelova sa sustavom SharePoint Server**</span><span class="sxs-lookup"><span data-stu-id="b11da-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="b11da-111">Web-dijelovi mogu se koristiti u modernim i klasičnim stranicama unutar lokalnih okruženja.</span><span class="sxs-lookup"><span data-stu-id="b11da-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="b11da-112">Dodatne informacije o modernim stranicama potražite u članku [Dodavanje sažetka sadržaja servisa Yammer na modernu stranicu u sustavu SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span><span class="sxs-lookup"><span data-stu-id="b11da-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="b11da-113">Dodatne informacije o klasičnim stranicama [potražite u članku Dodavanje sažetka sadržaja servisa Yammer klasičnoj stranici u sustavima SharePoint Servers 2013, 2016 i 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span><span class="sxs-lookup"><span data-stu-id="b11da-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="b11da-114">**Yammer ugrađivanje**</span><span class="sxs-lookup"><span data-stu-id="b11da-114">**Yammer Embed**</span></span>  

<span data-ttu-id="b11da-115">Pomoću alata Za ugradnju konfiguracije testirajte upotrebu ugradnje.</span><span class="sxs-lookup"><span data-stu-id="b11da-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="b11da-116">Buduće ažuriranje za ugradi omogućit će novi doživljaj servisa Yammer.</span><span class="sxs-lookup"><span data-stu-id="b11da-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="b11da-117">Dodatne informacije potražite u [alatu za konfiguraciju ugradnje servisa Yammer](https://aka.ms/YammerEmbedConfigureTool).</span><span class="sxs-lookup"><span data-stu-id="b11da-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="b11da-118">Da biste bolje razumjeli komponentu Yammer Embed, [pročitajte odjeljak Ugrađivanje sažetka sadržaja](https://aka.ms/YammerDevDocs).</span><span class="sxs-lookup"><span data-stu-id="b11da-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="b11da-119">**Poznati problemi i ograničenja**</span><span class="sxs-lookup"><span data-stu-id="b11da-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="b11da-120">ID-ovi grupa nisu dostupni u novim URL-ovima servisa Yammer koji su se promijenili.</span><span class="sxs-lookup"><span data-stu-id="b11da-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="b11da-121">Vratite se u klasični način rada da biste dobili ID-ove grupe ili druge ID-ove iz URL-ova.</span><span class="sxs-lookup"><span data-stu-id="b11da-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="b11da-122">Prilagođene (ispraznosti) domene nisu podržane.</span><span class="sxs-lookup"><span data-stu-id="b11da-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="b11da-123">Yammer Embed nije optimiziran za mobilne uređaje.</span><span class="sxs-lookup"><span data-stu-id="b11da-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="b11da-124">Koristite moderne stranice s web-dijelom Razgovori za Yammer za najbolji doživljaj.</span><span class="sxs-lookup"><span data-stu-id="b11da-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="b11da-125">Prilagođene teme mogu utjecati na izgled i upotrebljivost web-dijela razgovora servisa Yammer.</span><span class="sxs-lookup"><span data-stu-id="b11da-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="b11da-126">Otvorite slučaj podrške da biste prijavili probleme.</span><span class="sxs-lookup"><span data-stu-id="b11da-126">Open a support case to report issues.</span></span>