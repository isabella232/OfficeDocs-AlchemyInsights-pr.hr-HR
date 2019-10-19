---
title: Zamijenite svoju klasični root stranicu s modernim stranicama
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749252"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="992e6-102">Zamijenite svoju klasični root stranicu s modernim stranicama</span><span class="sxs-lookup"><span data-stu-id="992e6-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="992e6-103">Ako je vaša okolina postavljena prije travnja 2019, možete promijeniti korijensko web-mjesto na moderno web-mjesto pomoću Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="992e6-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="992e6-104">Ako imate drugo web-mjesto koje želite koristiti kao root web-mjesto, možete zamijeniti [(swap) root web-mjesto](https://docs.microsoft.com/sharepoint/modern-root-site) s njom.</span><span class="sxs-lookup"><span data-stu-id="992e6-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="992e6-105">Pomoću poziva [-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zamijenite mjesto web-mjesta s drugim web-mjestom dok arhivirate originalno web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="992e6-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="992e6-106">Dostupno i za timsko web-mjesto (nije povezano s grupom) i web-mjesto komunikacije.</span><span class="sxs-lookup"><span data-stu-id="992e6-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="992e6-107">Uskoro će se uvesti dodatne mogućnosti koje će vam omogućiti da nastavite koristiti sadržaj na web-mjestu, ali pretvorite postojeće web-mjesto na web-mjesto komunikacije.</span><span class="sxs-lookup"><span data-stu-id="992e6-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="992e6-108">Ove mogućnosti će se postupno isvaljivati.</span><span class="sxs-lookup"><span data-stu-id="992e6-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="992e6-109">Nastavite provjeriti Office 365 Message Center za ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="992e6-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="992e6-110">Poznati problemi s zamjene web-mjesta</span><span class="sxs-lookup"><span data-stu-id="992e6-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="992e6-111">Ciljno web-mjesto može vratiti pogrešku "nije pronađeno" (HTTP 404) u kratkom vremenskom razdoblju.</span><span class="sxs-lookup"><span data-stu-id="992e6-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="992e6-112">Sadržaj će se morati obnoviti za ažuriranje indeksa pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="992e6-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="992e6-113">Nema ručnog koraka potreban-to će biti učinjeno automatski.</span><span class="sxs-lookup"><span data-stu-id="992e6-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="992e6-114">Sve što ovisi o "statičkim" vezama (kao što su datoteka Sync i OneNote datoteke) morat će se ručno ispraviti.</span><span class="sxs-lookup"><span data-stu-id="992e6-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="992e6-115">Ako je izvorna web-lokacija web-mjesta interesne grupe, ažurirajte URL.</span><span class="sxs-lookup"><span data-stu-id="992e6-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="992e6-116">Nabavite popis svih web-mjesta organizacijskih vijesti.</span><span class="sxs-lookup"><span data-stu-id="992e6-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="992e6-117">Možda će biti potrebno provjeriti web-mjesta Project Servera kako bi se osiguralo da su još uvijek ispravno povezane.</span><span class="sxs-lookup"><span data-stu-id="992e6-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





