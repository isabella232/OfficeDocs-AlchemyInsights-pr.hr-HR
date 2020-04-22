---
title: Pristup uslugama umirovljenja
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687250"
---
# <a name="access-services-retirement"></a><span data-ttu-id="55736-102">Pristup uslugama umirovljenja</span><span class="sxs-lookup"><span data-stu-id="55736-102">Access services retirement</span></span>

<span data-ttu-id="55736-103">Kao što smo prvotno najavili u MC97576, u ožujku 2017., i nastavili komunicirati tijekom protekle godine, usluge pristupa se umirovi.</span><span class="sxs-lookup"><span data-stu-id="55736-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="55736-104">Sljedeća faza u ovom procesu bit će uklanjanje web-baza podataka programa Access koje koriste SharePoint popise kao njihovu temeljnu pohranu podataka.</span><span class="sxs-lookup"><span data-stu-id="55736-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="55736-105">**Kako to utječe na mene?**</span><span class="sxs-lookup"><span data-stu-id="55736-105">**How does this affect me?**</span></span>

<span data-ttu-id="55736-106">Počevši od lipnja 2019.</span><span class="sxs-lookup"><span data-stu-id="55736-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="55736-107">**Što trebam učiniti kako bih se pripremio za ovu promjenu?**</span><span class="sxs-lookup"><span data-stu-id="55736-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="55736-108">Preporučujemo vam da stvorite plan prijelaza za web-baze podataka programa Access vaše tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="55736-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="55736-109">Administratori mogu koristiti [skener aplikacija programa SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) za dobivanje zaliha aplikacija programa Access koje web-mjesta koriste.</span><span class="sxs-lookup"><span data-stu-id="55736-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="55736-110">Postoji nekoliko načina migracije podataka web-baza podataka programa Access:</span><span class="sxs-lookup"><span data-stu-id="55736-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="55736-111">Uvoz u lokalnu bazu podataka programa Access (. ACCDB) ili u Excel datoteku.</span><span class="sxs-lookup"><span data-stu-id="55736-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="55736-112">Preporučujemo i da Microsoft PowerApps bude alternativna platforma za stvaranje poslovnih rješenja bez koda za web i mobilne uređaje.</span><span class="sxs-lookup"><span data-stu-id="55736-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>