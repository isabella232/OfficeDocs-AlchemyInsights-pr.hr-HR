---
title: Ograničavanje sustava tijekom migracije servisa SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "9000353"
- "1987"
- "9000136"
- "2968"
ms.assetid: ''
ms.openlocfilehash: dc77c462fcf32817c92709852e2d03ab2086b9a4
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958890"
---
# <a name="sharepoint-throttling"></a><span data-ttu-id="ff324-102">Ograničavanje sustava servisa SharePoint</span><span class="sxs-lookup"><span data-stu-id="ff324-102">SharePoint throttling</span></span>

<span data-ttu-id="ff324-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="ff324-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ff324-104">**Ograničavanje servisa SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="ff324-104">**SharePoint Online throttling**</span></span>

<span data-ttu-id="ff324-105">SharePoint Online koristi ograničavanje za održavanje optimalnih performansi i pouzdanosti servisa SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="ff324-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="ff324-106">Ograničavanjem se ograničava broj korisničkih radnji ili istodobnih poziva (skriptom ili kodom) radi sprječavanja prekomjernog korištenja resursa.</span><span class="sxs-lookup"><span data-stu-id="ff324-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span>

<span data-ttu-id="ff324-107">Da biste saznali više, posjetite poveznice u nastavku:</span><span class="sxs-lookup"><span data-stu-id="ff324-107">For more information please visit the links below:</span></span>

- [<span data-ttu-id="ff324-108">Izbjegavanje uskih grla ili blokiranja u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ff324-108">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)
- [<span data-ttu-id="ff324-109">Migracija podataka i ograničavanje SPO-a</span><span class="sxs-lookup"><span data-stu-id="ff324-109">Data Migration and SPO Throttling</span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)
- [<span data-ttu-id="ff324-110">Brzina migracije sustava SharePoint Online i OneDrive</span><span class="sxs-lookup"><span data-stu-id="ff324-110">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
- [<span data-ttu-id="ff324-111">Rukovanje ograničavanjem sustava SharePoint Online korištenjem eksponencijalnog udaljavanja </span><span class="sxs-lookup"><span data-stu-id="ff324-111">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
- [<span data-ttu-id="ff324-112">Planiranje kapaciteta i testiranje učitavanja u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ff324-112">Capacity planning and load testing SharePoint Online</span></span>](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)
- [<span data-ttu-id="ff324-113">Tijekom migracije doživljavam loše performanse ili ograničavanje</span><span class="sxs-lookup"><span data-stu-id="ff324-113">I am experiencing poor performance or throttling during migration</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting)