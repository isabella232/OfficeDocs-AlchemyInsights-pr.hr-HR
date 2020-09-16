---
title: Upravljanje shemom pretraživanja u sustavu SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770543"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="b87f7-102">Upravljanje shemom pretraživanja u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b87f7-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="b87f7-103">Shema pretraživanja kontrolira ono što korisnici mogu pretraživati, kako ga korisnici mogu pretraživati te kako možete prikazati rezultate na web-mjestima za pretraživanje.</span><span class="sxs-lookup"><span data-stu-id="b87f7-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="b87f7-104">Pročitajte članak [Upravljanje shemom pretraživanja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) da biste naučili kako:</span><span class="sxs-lookup"><span data-stu-id="b87f7-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="b87f7-105">Promijenite shemu pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="b87f7-105">Change the search schema.</span></span>
- <span data-ttu-id="b87f7-106">Stvaranje upravljanih svojstava</span><span class="sxs-lookup"><span data-stu-id="b87f7-106">Create managed properties.</span></span>
- <span data-ttu-id="b87f7-107">Preslikavanje svojstva pretražena radi indeksiranja na upravljana svojstva.</span><span class="sxs-lookup"><span data-stu-id="b87f7-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="b87f7-108">Uočite sljedeće u odnosu na upravljanje shemom pretraživanja:</span><span class="sxs-lookup"><span data-stu-id="b87f7-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="b87f7-109">Ako primite upozorenje **u kojem se navodi da je aplikacija pauziran** prilikom promjene sheme, to je samo privremeno budući da se odvija održavanje servisa.</span><span class="sxs-lookup"><span data-stu-id="b87f7-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="b87f7-110">Ako je prošlo više od 24 sata, a vi i dalje nailite na upozorenje, prijavite slučaj podrške.</span><span class="sxs-lookup"><span data-stu-id="b87f7-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="b87f7-111">Kada promijenite upravljana svojstva ili dodate nove, promjene će se primijeniti samo nakon ponovnog pretraživanja sadržaja.</span><span class="sxs-lookup"><span data-stu-id="b87f7-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="b87f7-112">U sustavu SharePoint online pretraživanje radi indeksiranja automatski se odvija na temelju definiranog rasporeda pretraživanja radi indeksiranja.</span><span class="sxs-lookup"><span data-stu-id="b87f7-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="b87f7-113">Da biste bili sigurni da su vaše promjene pretražena radi indeksiranja, možete posebno [zatražiti ponovno indeksiranje popisa ili biblioteke](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="b87f7-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="b87f7-114">Potpuni pregled sheme pretraživanja potražite u članku [uvođenje sheme pretraživanja](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="b87f7-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


