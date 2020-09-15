---
title: Swap svoje klasično korijensko web-mjesto s modernim web-mjestom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691171"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="4122a-102">Swap svoje klasično korijensko web-mjesto s modernim web-mjestom</span><span class="sxs-lookup"><span data-stu-id="4122a-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="4122a-103">Ako je okruženje postavljeno prije travnja 2019, korijensko web-mjesto možete promijeniti na moderno web-mjesto pomoću komponente Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="4122a-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="4122a-104">Ako imate drugo web-mjesto koje želite koristiti kao korijensko web-mjesto, pomoću nje možete zamijeniti [(swap) korijensko web-mjesto](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="4122a-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="4122a-105">Pomoću poziva [-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) mijenjate mjesto web-mjesta s drugim web-mjestom tijekom arhiviranja izvornog web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="4122a-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="4122a-106">Dostupno za obje timsko web-mjesto (nije povezano s grupom) i komunikacijskim web-mjestom.</span><span class="sxs-lookup"><span data-stu-id="4122a-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="4122a-107">Uskoro će biti uvedene dodatne mogućnosti koje će vam dopustiti da nastavite koristiti sadržaj na web-mjestu, ali da biste postojeće web-mjesto pretvorili u komunikacijsko web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="4122a-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="4122a-108">Te će se mogućnosti postupno izkotrljali.</span><span class="sxs-lookup"><span data-stu-id="4122a-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="4122a-109">Nastavite provjeravati centar za poruke radi ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="4122a-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="4122a-110">Poznati problemi s zamjenom web-mjesta</span><span class="sxs-lookup"><span data-stu-id="4122a-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="4122a-111">Odredišno web-mjesto može u kratkom vremenskom periodu vratiti pogrešku "nije pronađeno" (HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="4122a-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="4122a-112">Sadržaj će se morati ponovno vratiti da bi se ažurirao indeks pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="4122a-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="4122a-113">Nije potreban ručni korak – to će se obaviti automatski.</span><span class="sxs-lookup"><span data-stu-id="4122a-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="4122a-114">Sve što ovisi o "statički" vezama (kao što su sinkronizacija datoteka i datoteke programa OneNote) morat će se ručno ispraviti.</span><span class="sxs-lookup"><span data-stu-id="4122a-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="4122a-115">Ako je izvorišno mjesto bilo organizacijsko web-mjesto vijesti, ažurirajte URL.</span><span class="sxs-lookup"><span data-stu-id="4122a-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="4122a-116">Nabavite popis svih web-mjesta organizacijskih vijesti.</span><span class="sxs-lookup"><span data-stu-id="4122a-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="4122a-117">Web-mjesta projektnog poslužitelja možda će se morati potvrditi da bi se osiguralo da su i dalje ispravno povezani.</span><span class="sxs-lookup"><span data-stu-id="4122a-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
