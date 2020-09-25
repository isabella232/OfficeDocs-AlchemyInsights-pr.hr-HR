---
title: alat za izvoz u programu Idiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277947"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="54313-102">Nije moguće instalirati ili pokrenuti alat za izvoz programa Idiscovery?</span><span class="sxs-lookup"><span data-stu-id="54313-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="54313-103">Ako ne možete instalirati ili pokrenuti alat za izvoz programa Idiscovery da biste preuzeli rezultate pretraživanja, provjerite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="54313-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="54313-104">Računalo koje koristite ispunjava te preduvjete:</span><span class="sxs-lookup"><span data-stu-id="54313-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="54313-105">32 ili 64-bitne verzije sustava Windows 7 i novije verzije</span><span class="sxs-lookup"><span data-stu-id="54313-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="54313-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="54313-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="54313-107">Podržani preglednik:</span><span class="sxs-lookup"><span data-stu-id="54313-107">A supported browser:</span></span>

  - <span data-ttu-id="54313-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="54313-108">Microsoft Edge</span></span>

    <span data-ttu-id="54313-109">Ili</span><span class="sxs-lookup"><span data-stu-id="54313-109">Or</span></span>

  - <span data-ttu-id="54313-110">Internet Explorer 10 i novije verzije</span><span class="sxs-lookup"><span data-stu-id="54313-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="54313-111">Drugi preglednici, kao što su Google Chrome i Mozilla Firefox, nisu podržani.</span><span class="sxs-lookup"><span data-stu-id="54313-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="54313-112">Vaša tvrtka ili ustanova može se povezati s krajnjom točkom u servisu Azure, što je \*\* \* . blob.Core.Windows.net\*\* (zamjenski znak predstavlja jedinstveni identifikator za vaš rad na izvozu).</span><span class="sxs-lookup"><span data-stu-id="54313-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="54313-113">U centru za sigurnost sustava Microsoft 365 dodeljen vam je izvoznu ulogu &amp; .</span><span class="sxs-lookup"><span data-stu-id="54313-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="54313-114">Ta je uloga prema zadanim postavkama dodijeljena samo grupi uloga upravitelja programa isdiscovery.</span><span class="sxs-lookup"><span data-stu-id="54313-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="54313-115">Pročitajte članak [Dodjela dozvola za otkrivanje iotkrivanja](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="54313-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="54313-116">Dodatne informacije potražite u članku [Izvoz rezultata pretraživanja sadržaja](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="54313-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="54313-117">Ako izvozite više od 100K poštanskih sandučića, morat ćete koristiti sljedeću PowerShell da biste preuzeli rezultate izvoza:  [Izvoz rezultata iz više od 100k poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="54313-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>