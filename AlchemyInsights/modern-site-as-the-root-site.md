---
title: Moderna stranica kao root stranice
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054694"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="0bbc0-102">Moderna stranica kao root stranice</span><span class="sxs-lookup"><span data-stu-id="0bbc0-102">Modern site as root site</span></span>

<span data-ttu-id="0bbc0-103">Započeli smo s uvođenju nove značajke koja će vam omogućiti da [zamijenite svoje klasično web-mjesto root stranicu s modernim stranicama](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="0bbc0-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="0bbc0-104">Pomoću poziva [-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zamijenite mjesto web-mjesta s drugim web-mjestom dok arhivirate originalno web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="0bbc0-105">Dostupno i za timsko web-mjesto (nije povezano s grupom) i web-mjesto komunikacije.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="0bbc0-106">Nemojte brisati klasični root web stranice za stvaranje moderne komunikacijske stranice.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="0bbc0-107">Microsoft ne podržava to.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="0bbc0-108">Brisanjem korijenskog web-mjesta sve će SharePoint web-mjesta u vašoj organizaciji biti nedostupne svim korisnicima, sve dok ne vratite web-mjesto ili stvorite novo web-mjesto na istom URL-u.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="0bbc0-109">Mi ćemo komunicirati ovu značajku putem centra za poruke.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="0bbc0-110">Trebali biste očekivati da će značajka biti uključena u vašeg stanara uskoro.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="0bbc0-111">Poznati problemi s zamjene web-mjesta</span><span class="sxs-lookup"><span data-stu-id="0bbc0-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="0bbc0-112">Ciljno web-mjesto može vratiti pogrešku "nije pronađeno" (HTTP 404) u kratkom vremenskom razdoblju.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="0bbc0-113">Sadržaj će se morati obnoviti za ažuriranje indeksa pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="0bbc0-114">Ovdje nije potreban ručni korak, to će biti učinjeno automatski.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="0bbc0-115">Sve što ovisi o "statičkim" vezama (kao što su datoteka Sync i OneNote datoteke) morat će se ručno ispraviti.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="0bbc0-116">Možda će biti potrebno provjeriti web-mjesta Project Servera kako bi se osiguralo da su još uvijek ispravno povezane.</span><span class="sxs-lookup"><span data-stu-id="0bbc0-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
