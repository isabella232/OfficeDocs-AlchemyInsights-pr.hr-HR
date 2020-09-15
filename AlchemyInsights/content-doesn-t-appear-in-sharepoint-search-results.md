---
title: Sadržaj se ne prikazuje u rezultatima pretraživanja sustava SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713122"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="3b7f0-102">Sadržaj se ne prikazuje u rezultatima pretraživanja sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="3b7f0-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="3b7f0-103">Slijedite ove korake za otklanjanje poteškoća kada se očekivani sadržaj ne prikazuje u rezultatima pretraživanja:</span><span class="sxs-lookup"><span data-stu-id="3b7f0-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="3b7f0-104">Provjerite je li **web-mjesto** koje sadrži očekivani sadržaj postavljeno tako da dopušta prikaz sadržaja u rezultatima pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="3b7f0-105">Slijedite korake u članku [Prikaz sadržaja na web-mjestu u rezultatima pretraživanja](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="3b7f0-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="3b7f0-106">Provjerite je li **popis** ili **Biblioteka** koja sadrži očekivani sadržaj postavljena tako da omogućuje prikaz sadržaja u rezultatima pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="3b7f0-107">Slijedite korake u odjeljku [Prikaz sadržaja s popisa ili biblioteka u rezultatima pretraživanja](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="3b7f0-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="3b7f0-108">Provjerite je li stranica, dokument ili prilagođeni prikaz stranice objavljen kao **glavna verzija.**</span><span class="sxs-lookup"><span data-stu-id="3b7f0-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="3b7f0-109">Slijedeći korak 3 u [pretraživanju ne vraća sve rezultate u sustavu SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="3b7f0-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="3b7f0-110">Provjerite ima li korisnik **dozvolu** za prikaz sadržaja.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="3b7f0-111">Slijedite korake u članku [razumijevanje razina dozvola u sustavu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="3b7f0-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="3b7f0-112">Ako je shema pretraživanja izmijenjena dodavanjem novog upravljanog svojstva uređivanjem upravljanog svojstva ili uklanjanjem upravljanog svojstva, zatražiće se mogućnost pretraživanja radi indeksiranja i ponovnog indeksa.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="3b7f0-113">**Ponovno Indeksirajte** sadržaj slijedeći korake u odjeljku [ručno zahtjev za indeksiranje i ponovnim indeksiranjem web-mjesta, biblioteke ili popisa](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="3b7f0-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="3b7f0-114">To bi moglo potrajati, čekati 24 sata prije nego što ponovno provjerite rezultate.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="3b7f0-115">Dodatne informacije potražite u članku [Omogućivanje pretraživanja sadržaja na web-mjestu](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="3b7f0-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
