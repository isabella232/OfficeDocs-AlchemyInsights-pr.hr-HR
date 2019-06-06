---
title: Upravljanje pretraživanja rječnika u SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736045"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="20901-102">Pretraživanje u programu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="20901-102">Search in SharePoint Online</span></span>

<span data-ttu-id="20901-103">Sadržaj mora pretražiti radi indeksiranja i dodati indeks pretraživanja za korisnike da biste pronašli što oni tražite u SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="20901-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="20901-104">Sadržaj automatski pretražuje na temelju rasporedu unaprijed definiranih pretraživanja radi indeksiranja (rasporeda pretraživanja radi indeksiranja sadržaja ne može se mijenjati).</span><span class="sxs-lookup"><span data-stu-id="20901-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="20901-105">Pretraživač uzima sadržaj koji je promijenjen od posljednjeg pretraživanja i ažurira indeks.</span><span class="sxs-lookup"><span data-stu-id="20901-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="20901-106">Da biste osigurali radi indeksiranja sadržaja i ažuriranje indeksa, slijedite dolje navedene korake.</span><span class="sxs-lookup"><span data-stu-id="20901-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="20901-107">Provjerite sadržaj možete pronaći izradom sadržaja web-mjesta koji se može pretraživati.</span><span class="sxs-lookup"><span data-stu-id="20901-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="20901-108">Za dodatne informacije pogledajte [Omogući sadržaj na web-mjestu mogu se pretraživati](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="20901-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="20901-109">Kada ste promijenili upravljano svojstvo ili kada ste promijenili mapiranje pretražena radi indeksiranja i upravljanih svojstava, web-mjesta mora biti ponovno pretražena radi indeksiranja sadržaja prije promjene odrazit će se u indeksu pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="20901-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="20901-110">Jer vaše se promjene u shemi pretraživanja i indeksiranja će da ne stvarnog web-mjesta neće automatski ponovno indeksirati web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="20901-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="20901-111">Za dodatne informacije pogledajte [ručno zahtjev za pretraživanje radi indeksiranja i ponovno indeksiranje web-mjesta u biblioteku ili popis](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="20901-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="20901-112">Pričekajte barem 24 sata nakon ručno zahtijevanje pretraživanja radi indeksiranja sadržaja i puni ponovno indeksirati da biste vidjeli Ako još uvijek imate problema.</span><span class="sxs-lookup"><span data-stu-id="20901-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="20901-113">Ako više od 24 sata prošlo otkad je inicirao pretraživanja radi indeksiranja sadržaja i puni ponovno indeksirati, prijaviti podršku slučaj.</span><span class="sxs-lookup"><span data-stu-id="20901-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="20901-114">U mnogim slučajevima smo već radite rješenje.</span><span class="sxs-lookup"><span data-stu-id="20901-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="20901-115">Molimo pošaljite nam najmanje 24 sata dovršiti rješenje.</span><span class="sxs-lookup"><span data-stu-id="20901-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="20901-116">**Važno**: Ako web-mjesto, dokument (biblioteka) ili popis je izbrisana i još uvijek prikazuje u rezultatima pretraživanja, korisnici trebaju primati pojavila pogreška 404 datoteka nije pronađena kada pokušavate pristupiti.</span><span class="sxs-lookup"><span data-stu-id="20901-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="20901-117">Taj problem treba prijavljeni kao slučaj podršku za daljnje istraživanja.</span><span class="sxs-lookup"><span data-stu-id="20901-117">This issue should be logged as a support case for further investigation.</span></span> 



