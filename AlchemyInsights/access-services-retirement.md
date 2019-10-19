---
title: Pristup uslugama umirovljenja
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747776"
---
# <a name="access-services-retirement"></a><span data-ttu-id="48c86-102">Pristup uslugama umirovljenja</span><span class="sxs-lookup"><span data-stu-id="48c86-102">Access services retirement</span></span>

<span data-ttu-id="48c86-103">Kao što smo prvotno najavili u MC97576, u ožujku 2017, i nastavio komunicirati tijekom protekle godine Accessove usluge su umirovljene iz Office 365.</span><span class="sxs-lookup"><span data-stu-id="48c86-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="48c86-104">Sljedeća faza u ovom procesu će biti uklanjanje Access web baze podataka koje koriste SharePoint popise kao njihove temeljne pohrane podataka.</span><span class="sxs-lookup"><span data-stu-id="48c86-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="48c86-105">**Kako to utječe na mene?**</span><span class="sxs-lookup"><span data-stu-id="48c86-105">**How does this affect me?**</span></span>

<span data-ttu-id="48c86-106">Počevši od lipnja 2019, zaustavit ćemo stvaranje novih baza podataka programa Access u sustavu SharePoint online i isključiti uslugu i sve preostale aplikacije do travnja 2020.</span><span class="sxs-lookup"><span data-stu-id="48c86-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="48c86-107">**Što trebam učiniti kako bih se pripremio za ovu promjenu?**</span><span class="sxs-lookup"><span data-stu-id="48c86-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="48c86-108">Potičemo vas da stvorite plan prijelaza za web-baze podataka programa Access vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="48c86-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="48c86-109">Administratori mogu koristiti [skener aplikacije SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) za dobivanje inventara aplikacija programa Access koje web-mjesta koriste.</span><span class="sxs-lookup"><span data-stu-id="48c86-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="48c86-110">Postoji nekoliko načina Migriranje podataka web-baze programa Access:</span><span class="sxs-lookup"><span data-stu-id="48c86-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="48c86-111">Uvoz u lokalnu bazu podataka programa Access (. ACCDB) ili u Excelovu datoteku.</span><span class="sxs-lookup"><span data-stu-id="48c86-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="48c86-112">Preporučujemo i istraživanje Microsoft PowerApps kao alternativne platforme za stvaranje nekôda poslovnih rješenja za web i mobilne uređaje.</span><span class="sxs-lookup"><span data-stu-id="48c86-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>