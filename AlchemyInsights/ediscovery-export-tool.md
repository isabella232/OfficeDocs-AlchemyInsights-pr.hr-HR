---
title: Alat za izvoz elektroničkih predočavanja elektroničkih elektroničkih podataka
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814580"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="9893d-102">Ne možete instalirati ili pokrenuti alat za izvoz predočavanja elektroničkih podataka?</span><span class="sxs-lookup"><span data-stu-id="9893d-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="9893d-103">Ako ne možete instalirati ili pokrenuti alat za izvoz e-otkrivanja da biste preuzeli rezultate pretraživanja, provjerite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="9893d-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="9893d-104">Računalo koje koristite zadovoljava sljedeće preduvjete:</span><span class="sxs-lookup"><span data-stu-id="9893d-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="9893d-105">32-bitne ili 64-bitne verzije sustava Windows 7 i novije verzije</span><span class="sxs-lookup"><span data-stu-id="9893d-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="9893d-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="9893d-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="9893d-107">Podržani preglednik:</span><span class="sxs-lookup"><span data-stu-id="9893d-107">A supported browser:</span></span>

  - <span data-ttu-id="9893d-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="9893d-108">Microsoft Edge</span></span>

    <span data-ttu-id="9893d-109">Ili</span><span class="sxs-lookup"><span data-stu-id="9893d-109">Or</span></span>

  - <span data-ttu-id="9893d-110">Internet Explorer 10 i novije verzije</span><span class="sxs-lookup"><span data-stu-id="9893d-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="9893d-111">Drugi preglednici, kao što su Google Chrome i Mozilla Firefox, nisu podržani.</span><span class="sxs-lookup"><span data-stu-id="9893d-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="9893d-112">Vaša tvrtka ili ustanova može se povezati s krajnjom tonom na servisu Azure, **\* a to je .blob.core.windows.net** (zamjenski znak predstavlja jedinstveni identifikator za posao izvoza).</span><span class="sxs-lookup"><span data-stu-id="9893d-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="9893d-113">Uloga Izvoz dodijeljena vam je u centru za sigurnosnu usklađenost sustava Microsoft 365. &amp;</span><span class="sxs-lookup"><span data-stu-id="9893d-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="9893d-114">Ta se uloga po zadanom dodjeljuje samo grupi uloga upravitelja predočavanja elektroničkih elektroničkih obveza.</span><span class="sxs-lookup"><span data-stu-id="9893d-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="9893d-115">Pogledajte [dodjela dozvola za predočavanje elektroničkih datoteka](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="9893d-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="9893d-116">Dodatne informacije potražite u članku Izvoz [rezultata pretraživanja sadržaja](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="9893d-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="9893d-117">Ako izvozite više od 100 K poštanskih sandučića, morat ćete koristiti sljedeću ljusku Powershell da biste preuzeli rezultate izvoza: izvoz rezultata iz više  [od 100K poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="9893d-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>