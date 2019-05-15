---
title: Access services umirovljenje
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973904"
---
# <a name="access-services-retirement"></a><span data-ttu-id="60f2a-102">Access services umirovljenje</span><span class="sxs-lookup"><span data-stu-id="60f2a-102">Access services retirement</span></span>

<span data-ttu-id="60f2a-103">Kao smo izvorno najavio u MC97576, u 2017 Ožujak i nastavlja komunikaciju putem prošle godine Access Services u mirovini su se iz Office 365.</span><span class="sxs-lookup"><span data-stu-id="60f2a-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="60f2a-104">Sljedeće faze ovaj proces će biti uklanjanje pristup web-baze podataka koje koriste SharePoint popise kao njihove podlozi pohranu podataka.</span><span class="sxs-lookup"><span data-stu-id="60f2a-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="60f2a-105">Kako to utječe na mene?</span><span class="sxs-lookup"><span data-stu-id="60f2a-105">How does this affect me?</span></span>

<span data-ttu-id="60f2a-106">Početni lipanj 2019 ćemo će zaustaviti stvaranje nove baze podataka programa Access u SharePoint Online i isključi servis i sve preostale apps po 2020 Travanj.</span><span class="sxs-lookup"><span data-stu-id="60f2a-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="60f2a-107">Što je potrebno učiniti da biste pripremili za ovu promjenu?</span><span class="sxs-lookup"><span data-stu-id="60f2a-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="60f2a-108">Pozivamo vas da stvorite plan tranzicije za vaša organizacija pristup web-baze podataka.</span><span class="sxs-lookup"><span data-stu-id="60f2a-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="60f2a-109">Administratori možete koristiti [pristup SharePoint app skener](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) da biste nabavili zaliha apps pristup koji koriste web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="60f2a-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="60f2a-110">Postoji nekoliko načina za migraciju podataka Access web baze podataka:</span><span class="sxs-lookup"><span data-stu-id="60f2a-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="60f2a-111">Uvoz lokalne baze podataka Access (. ACCDB) ili datoteku programa Excel.</span><span class="sxs-lookup"><span data-stu-id="60f2a-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="60f2a-112">Preporučujemo i istraživanje Microsoft PowerApps kao alternativni platforma za stvaranje rješenja bez koda poslovne za web i mobilnih uređaja.</span><span class="sxs-lookup"><span data-stu-id="60f2a-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>