---
title: Moderna stranica kao root site
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713783"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="2295f-102">Moderna stranica kao root site</span><span class="sxs-lookup"><span data-stu-id="2295f-102">Modern site as root site</span></span>

<span data-ttu-id="2295f-103">Počeli smo uvesti novu značajku koja će vam omogućiti da [zamijenite svoje klasične stranice root stranice s modernim stranicama](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="2295f-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="2295f-104">Koristite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) za zamjenu lokacije web-mjesta s drugim web-mjestom dok arhivijete izvornu web-lokaciju.</span><span class="sxs-lookup"><span data-stu-id="2295f-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="2295f-105">Dostupno za timsko web-mjesto (nije povezano s grupom) i komunikacijskom web-mjestu.</span><span class="sxs-lookup"><span data-stu-id="2295f-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="2295f-106">Nemojte brisati svoje klasične root stranice za stvaranje moderne komunikacijske stranice.</span><span class="sxs-lookup"><span data-stu-id="2295f-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="2295f-107">Microsoft to ne podržava.</span><span class="sxs-lookup"><span data-stu-id="2295f-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="2295f-108">Brisanjem korijenskog web-mjesta sva sharepoint web-mjesta u tvrtki ili ustanovi neće biti dostupna svim korisnicima dok ne vratite web-mjesto ili stvorite novo web-mjesto na istom URL-u.</span><span class="sxs-lookup"><span data-stu-id="2295f-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="2295f-109">Ovu ćemo značajku komunicirati putem centra za poruke.</span><span class="sxs-lookup"><span data-stu-id="2295f-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="2295f-110">Uskoro biste trebali očekivati da će značajka biti uključena u klijentu.</span><span class="sxs-lookup"><span data-stu-id="2295f-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="2295f-111">Poznati problemi s adut za zamjenu web-mjesta</span><span class="sxs-lookup"><span data-stu-id="2295f-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="2295f-112">Ciljno web-mjesto može vratiti pogrešku "nije pronađeno" (HTTP 404) na kratko vrijeme.</span><span class="sxs-lookup"><span data-stu-id="2295f-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="2295f-113">Sadržaj će se morati preistovjetnuti radi ažuriranja indeksa pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="2295f-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="2295f-114">Ovdje nije potreban ručni korak, to će se učiniti automatski.</span><span class="sxs-lookup"><span data-stu-id="2295f-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="2295f-115">Sve što ovisi o "statičkim" vezama (kao što su Sinkronizacija datoteka i onenote datoteka) morat će se ručno ispraviti.</span><span class="sxs-lookup"><span data-stu-id="2295f-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="2295f-116">Možda će biti potrebno provjeriti valjanost web-mjesta sustava Project Server da bi se osiguralo da su još uvijek ispravno pridružena.</span><span class="sxs-lookup"><span data-stu-id="2295f-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
