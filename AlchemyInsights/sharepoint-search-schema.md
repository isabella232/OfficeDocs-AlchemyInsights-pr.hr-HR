---
title: Upravljanje shemom pretraživanja u sustavu SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042955"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="c5b2e-102">Upravljanje shemom pretraživanja u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c5b2e-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="c5b2e-103">Shema pretraživanja kontrolira što korisnici mogu pretraživati, kako ga korisnici mogu pretraživati i kako možete predstaviti rezultate na web-lokacijama pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="c5b2e-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="c5b2e-104">Pogledajte [Upravljanje shemom pretraživanja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) da biste saznali kako:</span><span class="sxs-lookup"><span data-stu-id="c5b2e-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="c5b2e-105">Promijenite shemu pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="c5b2e-105">Change the search schema.</span></span>
- <span data-ttu-id="c5b2e-106">Stvorite upravljana svojstva.</span><span class="sxs-lookup"><span data-stu-id="c5b2e-106">Create managed properties.</span></span>
- <span data-ttu-id="c5b2e-107">Preslikavanje svojstava pretraženog radi indeksiranja u upravljana svojstva.</span><span class="sxs-lookup"><span data-stu-id="c5b2e-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="c5b2e-108">Imajte na umu sljedeće u vezi s upravljanjem shemom pretraživanja:</span><span class="sxs-lookup"><span data-stu-id="c5b2e-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="c5b2e-109">Ako primite upozorenje **u kojem se navodi da je aplikacija pauzirana** prilikom izrade promjene sheme, to je samo privremeno jer se pojavljuje održavanje servisa.</span><span class="sxs-lookup"><span data-stu-id="c5b2e-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="c5b2e-110">Ako je prošlo više od 24 sata i još uvijek osjetite upozorenje, prijavite se slučaj podrške.</span><span class="sxs-lookup"><span data-stu-id="c5b2e-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="c5b2e-111">Kada promijenite upravljana svojstva ili dodate nove, promjene će stupiti na snagu tek nakon ponovnog pretraživanja sadržaja.</span><span class="sxs-lookup"><span data-stu-id="c5b2e-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="c5b2e-112">U sustavu SharePoint online pretraživanje radi indeksiranja automatski se temelji na definiranom rasporedu pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="c5b2e-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="c5b2e-113">Da biste bili sigurni da su vaše promjene pretražene radi indeksiranja sadržaja, možete posebno [zatražiti ponovno indeksiranje popisa ili biblioteke](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="c5b2e-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="c5b2e-114">Potpuni pregled sheme pretraživanja potražite u članku [uvođenje sheme pretraživanja](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="c5b2e-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


