---
title: Sadržaj se ne prikazuje u rezultatima pretraživanja sustava SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705653"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="7d9e6-102">Sadržaj se ne prikazuje u rezultatima pretraživanja sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="7d9e6-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="7d9e6-103">Slijedite ove korake za otklanjanje poteškoća kada se očekivani sadržaj ne prikazuje u rezultatima pretraživanja:</span><span class="sxs-lookup"><span data-stu-id="7d9e6-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="7d9e6-104">Provjerite je li **web-mjesto** koje sadrži očekivani sadržaj postavljeno tako da omogućuje prikazivanje sadržaja u rezultatima pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="7d9e6-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="7d9e6-105">Slijedite korake u [odjeljku Prikaz sadržaja na web-mjestu u rezultatima pretraživanja](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="7d9e6-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="7d9e6-106">Provjerite je li **popis** ili **biblioteka** koja sadrži očekivani sadržaj postavljena tako da omogućuje prikazivanje sadržaja u rezultatima pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="7d9e6-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="7d9e6-107">Slijedite korake u odjeljku [Prikaz sadržaja s popisa ili biblioteka u rezultatima pretraživanja](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="7d9e6-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="7d9e6-108">Provjerite objavljuju li se izgled stranice, dokumenta ili prilagođene stranice kao **glavna verzija.**</span><span class="sxs-lookup"><span data-stu-id="7d9e6-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="7d9e6-109">Slijedite treći korak u [pretraživanju ne vraća sve rezultate u sustavu SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="7d9e6-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="7d9e6-110">Provjerite ima li korisnik **dozvole** za prikaz sadržaja.</span><span class="sxs-lookup"><span data-stu-id="7d9e6-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="7d9e6-111">Slijedite korake u članku [Razumijevanje razina dozvola u sustavu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="7d9e6-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="7d9e6-112">Ako je shema pretraživanja promijenjena dodavanjem novog upravljanog svojstva, uređivanjem upravljanog svojstva ili uklanjanjem upravljanog svojstva, bit će potrebno zatražiti pretraživanje radi indeksiranja sadržaja i ponovno indeksiranje.</span><span class="sxs-lookup"><span data-stu-id="7d9e6-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="7d9e6-113">**Ponovno indeksirajte** sadržaj slijedeći korake u odjeljku [Ručno traženje pretraživanja radi indeksiranja i ponovno indeksiranje web-mjesta, biblioteke ili popisa](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="7d9e6-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="7d9e6-114">To može potrajati, pričekajte 24 sata prije ponovnog provjere rezultata.</span><span class="sxs-lookup"><span data-stu-id="7d9e6-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="7d9e6-115">Dodatne informacije [potražite u odjeljku Omogućivanje pretraživanja sadržaja na web-mjestu](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="7d9e6-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
