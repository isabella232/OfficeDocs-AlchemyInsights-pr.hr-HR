---
title: Access services umirovljenje
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495743"
---
# <a name="access-services-retirement"></a><span data-ttu-id="15d6e-102">Access services umirovljenje</span><span class="sxs-lookup"><span data-stu-id="15d6e-102">Access services retirement</span></span>

<span data-ttu-id="15d6e-103">Kao smo izvorno najavio u MC97576, u 2017 Ožujak i nastavlja komunikaciju putem prošle godine Access Services u mirovini su se iz Office 365.</span><span class="sxs-lookup"><span data-stu-id="15d6e-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="15d6e-104">Sljedeće faze ovaj proces će biti uklanjanje pristup web-baze podataka koje koriste SharePoint popise kao njihove podlozi pohranu podataka.</span><span class="sxs-lookup"><span data-stu-id="15d6e-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="15d6e-105">**Kako to utječe na mene?**</span><span class="sxs-lookup"><span data-stu-id="15d6e-105">**How does this affect me?**</span></span>

<span data-ttu-id="15d6e-106">Početni lipanj 2019 ćemo će zaustaviti stvaranje nove baze podataka programa Access u SharePoint Online i isključi servis i sve preostale apps po 2020 Travanj.</span><span class="sxs-lookup"><span data-stu-id="15d6e-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="15d6e-107">**Što je potrebno učiniti da biste pripremili za ovu promjenu?**</span><span class="sxs-lookup"><span data-stu-id="15d6e-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="15d6e-108">Pozivamo vas da stvorite plan tranzicije za vaša organizacija pristup web-baze podataka.</span><span class="sxs-lookup"><span data-stu-id="15d6e-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="15d6e-109">Administratori možete koristiti [pristup SharePoint app skener](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) da biste nabavili zaliha apps pristup koji koriste web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="15d6e-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="15d6e-110">Postoji nekoliko načina za migraciju podataka Access web baze podataka:</span><span class="sxs-lookup"><span data-stu-id="15d6e-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="15d6e-111">Uvoz lokalne baze podataka Access (. ACCDB) ili datoteku programa Excel.</span><span class="sxs-lookup"><span data-stu-id="15d6e-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="15d6e-112">Preporučujemo i istraživanje Microsoft PowerApps kao alternativni platforma za stvaranje rješenja bez koda poslovne za web i mobilnih uređaja.</span><span class="sxs-lookup"><span data-stu-id="15d6e-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>