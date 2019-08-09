---
title: Upravljanje sheme pretraživanja u SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f49195bec64f115063ccfb5256e27fbecd4a54f6
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270089"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="58ff6-102">Upravljanje sheme pretraživanja u SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="58ff6-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="58ff6-103">Sheme pretraživanja kontrolira što korisnici mogu pretraživati za, kako mu korisnici mogu pretraživati i kako prikazati rezultate pretraživanja web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="58ff6-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="58ff6-104">Pogledajte [Upravljanje sheme pretraživanja u SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) da biste saznali kako:</span><span class="sxs-lookup"><span data-stu-id="58ff6-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="58ff6-105">Promjena sheme pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="58ff6-105">Change the search schema.</span></span>
- <span data-ttu-id="58ff6-106">Stvorite upravljana svojstva.</span><span class="sxs-lookup"><span data-stu-id="58ff6-106">Create managed properties.</span></span>
- <span data-ttu-id="58ff6-107">Karta pretraženog radi indeksiranja karta svojstva pretražena radi indeksiranja u upravljana svojstva.</span><span class="sxs-lookup"><span data-stu-id="58ff6-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="58ff6-108">Imajte na umu sljedeće vas pozdravljamo za upravljanje sheme pretraživanja:</span><span class="sxs-lookup"><span data-stu-id="58ff6-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="58ff6-109">Ako primite upozorenje koja govori **pauzirano je aplikacija** kada promjena sheme, to je samo privremene kao usluga održavanja pojavljivanja.</span><span class="sxs-lookup"><span data-stu-id="58ff6-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="58ff6-110">Ako istekli su više od 24 sata, a i dalje nailazite upozorenje, prijavite slučaj podršku.</span><span class="sxs-lookup"><span data-stu-id="58ff6-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="58ff6-111">Kada promijenite upravljana svojstva ili dodati nove promjene stupiti na snagu tek nakon što je ponovno pretraženog radi indeksiranja sadržaja.</span><span class="sxs-lookup"><span data-stu-id="58ff6-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="58ff6-112">U SharePoint Online pretraživanje radi indeksiranja sadržaja se događa automatski na temelju rasporedu definirani pretraživanja radi indeksiranja.</span><span class="sxs-lookup"><span data-stu-id="58ff6-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="58ff6-113">Da biste bili sigurni da vaše promjene su pretražena radi indeksiranja sadržaja, možete posebno [zahtjev je ponovno indeksiranje popisa ili biblioteke](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="58ff6-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="58ff6-114">Potpuni pregled sheme pretraživanja potražite [Uvod u sheme pretraživanja](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="58ff6-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


