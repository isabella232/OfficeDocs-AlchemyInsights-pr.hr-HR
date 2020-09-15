---
title: Mirovina u programu Access Services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698638"
---
# <a name="access-services-retirement"></a><span data-ttu-id="9acc5-102">Mirovina u programu Access Services</span><span class="sxs-lookup"><span data-stu-id="9acc5-102">Access services retirement</span></span>

<span data-ttu-id="9acc5-103">Kao što smo prvobitno najavili u MC97576, u ožujku 2017, i nastavili smo komunicirati u prošloj godini programa Access Services su u mirovini.</span><span class="sxs-lookup"><span data-stu-id="9acc5-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="9acc5-104">Sljedeća faza u ovom postupku bit će uklanjanje web-baza podataka programa Access koja koristi popise sustava SharePoint kao njihovo spremište podataka u pozadini.</span><span class="sxs-lookup"><span data-stu-id="9acc5-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="9acc5-105">**Kako to utječe na mene?**</span><span class="sxs-lookup"><span data-stu-id="9acc5-105">**How does this affect me?**</span></span>

<span data-ttu-id="9acc5-106">Počevši od lipnja 2019, zaustavit ćemo stvaranje novih baza podataka programa Access u sustavu SharePoint online i isključivanje servisa i svih preostalih aplikacija do travnja 2020.</span><span class="sxs-lookup"><span data-stu-id="9acc5-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="9acc5-107">**Što je potrebno učiniti da biste se pripremili za ovu promjenu?**</span><span class="sxs-lookup"><span data-stu-id="9acc5-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="9acc5-108">Preporučujemo vam da stvorite plan tranzicije za web-baze podataka programa Access tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="9acc5-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="9acc5-109">Administratori mogu koristiti [skener aplikacija sustava SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) da bi nabavili inventar aplikacija programa Access koje koriste web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="9acc5-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="9acc5-110">Podaci za web-baze podataka programa Access mogu se migrirati na nekoliko načina:</span><span class="sxs-lookup"><span data-stu-id="9acc5-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="9acc5-111">Uvoz u lokalnu bazu podataka programa Access (. ACCDB) ili u datoteku programa Excel.</span><span class="sxs-lookup"><span data-stu-id="9acc5-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="9acc5-112">Preporučujemo i istraživanje Microsoft PowerApps kao alternativne platforme za stvaranje nekodova poslovnih rješenja za web i mobilne uređaje.</span><span class="sxs-lookup"><span data-stu-id="9acc5-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>