---
title: Pretraživanje u sustavu SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044035"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="a010f-102">Pretraživanje i indeksiranje sadržaja u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a010f-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="a010f-103">Sadržaj mora biti pretražen radi indeksiranja i dodan u indeks pretraživanja da bi korisnici pronašli ono što pretražuju u sustavu SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="a010f-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="a010f-104">Sadržaj se automatski pretražuje na temelju unaprijed definiranih rasporeda pretraživanja radi indeksiranja (raspored pretraživanja radi indeksiranja ne može se promijeniti).</span><span class="sxs-lookup"><span data-stu-id="a010f-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="a010f-105">Alat za indeksiranje preuzima sadržaj koji se promijenio od zadnjeg pretraživanja radi indeksiranja sadržaja i obnavlja indeks.</span><span class="sxs-lookup"><span data-stu-id="a010f-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="a010f-106">Da biste osigurali da je sadržaj pretraživan i da je indeks ažuriran, napominjemo sljedeće:</span><span class="sxs-lookup"><span data-stu-id="a010f-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="a010f-107">Provjerite je li sadržaj moguće pronaći tako da se [sadržaj web-mjesta može pretraživati](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="a010f-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="a010f-108">Kada ste promijenili upravljano svojstvo ili kada ste promijenili mapiranje pretraživanja i upravljanih svojstava, web-mjesto se mora ponovno pretraživati radi indeksiranja prije nego što se promjene odražavaju u indeksu pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="a010f-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="a010f-109">Budući da su vaše promjene napravljene u shemi pretraživanja, a ne na stvarnom web-mjestu, pretraživač neće automatski ponovno indeksirati web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="a010f-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="a010f-110">Za više informacija pogledajte [ručno zatražite pretraživanje i ponovno indeksiranje web-mjesta, biblioteke ili popisa](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="a010f-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="a010f-111">Pričekajte najmanje 24 sata nakon ručnog traženja pretraživanja radi indeksiranja i potpunog ponovnog indeksa da biste vidjeli imate li još uvijek problem.</span><span class="sxs-lookup"><span data-stu-id="a010f-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="a010f-112">Ako je prošlo više od 24 sata od kada ste pokrenuli pretraživanje radi indeksiranja i potpuno ponovno indeksiranje, prijavite slučaj podrške.</span><span class="sxs-lookup"><span data-stu-id="a010f-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="a010f-113">U mnogim slučajevima već radimo na rješenju.</span><span class="sxs-lookup"><span data-stu-id="a010f-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="a010f-114">Molim vas, dajte nam najmanje 24 sata da dovršimo rješenje.</span><span class="sxs-lookup"><span data-stu-id="a010f-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a010f-115">Ako je web-mjesto, dokument (biblioteka) ili popis izbrisan i još se prikazuje u rezultatima pretraživanja, korisnici bi trebali primiti **pogrešku 404 datoteka nije pronađena** prilikom pokušaja pristupa.</span><span class="sxs-lookup"><span data-stu-id="a010f-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="a010f-116">Taj bi problem trebao biti prijavljen kao slučaj podrške za daljnju istragu.</span><span class="sxs-lookup"><span data-stu-id="a010f-116">This issue should be logged as a support case for further investigation.</span></span> 



