---
title: Moderno web-mjesto kao korijensko web-mjesto
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666862"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="6a7ac-102">Moderno web-mjesto kao korijensko web-mjesto</span><span class="sxs-lookup"><span data-stu-id="6a7ac-102">Modern site as root site</span></span>

<span data-ttu-id="6a7ac-103">Započeli smo s prikazom nove značajke koja će vam dopustiti da [zamijenite svoje klasično korijensko web-mjesto s modernim web](https://docs.microsoft.com/sharepoint/modern-root-site)-mjestom.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="6a7ac-104">Pomoću poziva [-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) mijenjate mjesto web-mjesta s drugim web-mjestom tijekom arhiviranja izvornog web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="6a7ac-105">Dostupno za obje timsko web-mjesto (nije povezano s grupom) i komunikacijskim web-mjestom.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="6a7ac-106">Nemojte brisati klasično korijensko web-mjesto da biste stvorili moderno komunikacijsko web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="6a7ac-107">Microsoft ne podržava ovo.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="6a7ac-108">Brisanjem korijenskog web-mjesta svi će web-mjesta sustava SharePoint u vašoj tvrtki ili ustanovi biti nedostupne svim korisnicima dok ne vratite web-mjesto ili stvorite novo web-mjesto na istom URL-u.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="6a7ac-109">Ovu značajku Komunicirat ćemo putem centra za poruke.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="6a7ac-110">Morate očekivati da će značajka uskoro biti uključena u zakupcu.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="6a7ac-111">Poznati problemi s zamjenom web-mjesta</span><span class="sxs-lookup"><span data-stu-id="6a7ac-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="6a7ac-112">Odredišno web-mjesto može u kratkom vremenskom periodu vratiti pogrešku "nije pronađeno" (HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="6a7ac-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="6a7ac-113">Sadržaj će se morati ponovno vratiti da bi se ažurirao indeks pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="6a7ac-114">Ovdje nije potreban ručni korak, to će se obaviti automatski.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="6a7ac-115">Sve što ovisi o "statički" vezama (kao što su sinkronizacija datoteka i datoteke programa OneNote) morat će se ručno ispraviti.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="6a7ac-116">Web-mjesta projektnog poslužitelja možda će se morati potvrditi da bi se osiguralo da su i dalje ispravno povezani.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
