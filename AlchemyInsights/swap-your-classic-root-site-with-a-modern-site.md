---
title: Zamjena klasičnog korijenskog web-mjesta modernim web-mjestom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741536"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="7f659-102">Zamjena klasičnog korijenskog web-mjesta modernim web-mjestom</span><span class="sxs-lookup"><span data-stu-id="7f659-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="7f659-103">Ako je okruženje postavljeno prije travnja 2019., korijensko web-mjesto možete promijeniti na moderno web-mjesto pomoću komponente Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7f659-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="7f659-104">Ako imate drugu web-lokaciju koju želite koristiti kao root web-lokaciju, možete zamijeniti [(zamijeniti) korijensku stranicu](https://docs.microsoft.com/sharepoint/modern-root-site) s njom.</span><span class="sxs-lookup"><span data-stu-id="7f659-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="7f659-105">Koristite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) za zamjenu lokacije web-mjesta s drugim web-mjestom dok arhivijete izvornu web-lokaciju.</span><span class="sxs-lookup"><span data-stu-id="7f659-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="7f659-106">Dostupno za timsko web-mjesto (nije povezano s grupom) i komunikacijskom web-mjestu.</span><span class="sxs-lookup"><span data-stu-id="7f659-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="7f659-107">Uskoro će se uvesti dodatne mogućnosti koje će vam omogućiti da nastavite koristiti sadržaj na web-mjestu, ali pretvorite postojeće web-mjesto na komunikacijsko web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="7f659-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="7f659-108">Te će se mogućnosti postupno uvesti.</span><span class="sxs-lookup"><span data-stu-id="7f659-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="7f659-109">Nastavite provjeravati ima li u centru za poruke ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="7f659-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="7f659-110">Poznati problemi s adut za zamjenu web-mjesta</span><span class="sxs-lookup"><span data-stu-id="7f659-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="7f659-111">Ciljno web-mjesto može vratiti pogrešku "nije pronađeno" (HTTP 404) na kratko vrijeme.</span><span class="sxs-lookup"><span data-stu-id="7f659-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="7f659-112">Sadržaj će se morati preistovjetnuti radi ažuriranja indeksa pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="7f659-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="7f659-113">Nema ručnog koraka - to će se učiniti automatski.</span><span class="sxs-lookup"><span data-stu-id="7f659-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="7f659-114">Sve što ovisi o "statičkim" vezama (kao što su Sinkronizacija datoteka i onenote datoteka) morat će se ručno ispraviti.</span><span class="sxs-lookup"><span data-stu-id="7f659-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="7f659-115">Ako je izvorišno web-mjesto bilo organizacijsko web-mjesto za vijesti, ažurirajte URL.</span><span class="sxs-lookup"><span data-stu-id="7f659-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="7f659-116">Nabavite popis svih organizacijskih web-mjesta s novostima.</span><span class="sxs-lookup"><span data-stu-id="7f659-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="7f659-117">Možda će biti potrebno provjeriti valjanost web-mjesta sustava Project Server da bi se osiguralo da su još uvijek ispravno pridružena.</span><span class="sxs-lookup"><span data-stu-id="7f659-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
