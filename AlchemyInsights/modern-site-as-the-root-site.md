---
title: Moderna web-mjesta kao korijensko web-mjesto
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543845"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="11107-102">Moderna web-mjesta kao korijensko web-mjesto</span><span class="sxs-lookup"><span data-stu-id="11107-102">Modern site as root site</span></span>

<span data-ttu-id="11107-103">Ćemo imati počelo pripremati rollout nove značajke koje će vam omogućuju da zamijeni vaš klasični mjesta korijensko web-mjesto s Moderna web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="11107-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="11107-104">Koristite [Pozovite SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Zamijeni mjesto web-mjesta s drugog web-mjesta vrijeme arhiviranja izvornog web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="11107-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="11107-105">Dostupno za timskog web-mjesta (nije povezano s grupom) i komunikacije web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="11107-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="11107-106">Brisanje klasični korijensko web-mjesto za stvaranje Moderna komunikacije web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="11107-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="11107-107">Ovo je Microsoft ne podržava.</span><span class="sxs-lookup"><span data-stu-id="11107-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="11107-108">Brisanje korijenskog web-mjesta će napraviti sve SharePoint web-mjestima u vašoj organizaciji nedostupni na sve korisnike dok ne obnovite web-mjesto ili stvorite novo web-mjesto na URL-u istoj.</span><span class="sxs-lookup"><span data-stu-id="11107-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="11107-109">Ćete smo komunikaciji značajka putem centra za poruku.</span><span class="sxs-lookup"><span data-stu-id="11107-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="11107-110">Značajka biti uključen u vaše klijentske uskoro očekivati.</span><span class="sxs-lookup"><span data-stu-id="11107-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="11107-111">Poznati problemi s zamjene web-mjesta</span><span class="sxs-lookup"><span data-stu-id="11107-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="11107-112">Ciljno mjesto može vratiti "nije pronađen" Pogreška (HTTP 404) za kratkog vremenskog razdoblja.</span><span class="sxs-lookup"><span data-stu-id="11107-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="11107-113">Sadržaj će morati biti ponovno pretražiti da radi indeksiranja da biste ažurirali indeks pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="11107-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="11107-114">Postoji bez ručnog korak potreban ovdje, to će učiniti automatski.</span><span class="sxs-lookup"><span data-stu-id="11107-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="11107-115">Ništa zavise "statički" veze (poput datoteka sinkronizacije datoteka i OneNote) morat ćete ručno ispraviti.</span><span class="sxs-lookup"><span data-stu-id="11107-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="11107-116">Web-mjesta Project Server možda morati provjeriti da biste bili sigurni da su i dalje povezani ispravno.</span><span class="sxs-lookup"><span data-stu-id="11107-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
