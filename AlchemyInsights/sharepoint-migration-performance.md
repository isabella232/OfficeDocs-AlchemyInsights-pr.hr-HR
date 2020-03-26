---
title: Performanse migracije sustava ShairPoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931883"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="b9cc4-102">Performanse migracije sustava ShairPoint</span><span class="sxs-lookup"><span data-stu-id="b9cc4-102">SharePoint migration performance</span></span>

<span data-ttu-id="b9cc4-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokreću poslovne ključne aplikacije na servis koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b9cc4-104">To obuhvaća migraciju sadržaja, sprječavanje gubitka podataka (DLP) i rješenja za sigurnosno kopiranje.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b9cc4-105">Tijekom tih presedana poduzimamo korake da bi servisi sustava SharePoint Online i servisi OneDrive ostali iznimno raspoloživi i pouzdani za korisnike koji više nego ikad ovise o servisu u udaljenim radnim scenarijima.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b9cc4-106">Na temelju podrške tog cilja implementirali smo čvršća restriktivna ograničenja na pozadinske aplikacije (migracija, DLP i rješenja sigurnosnih kopija) tijekom radnog dana.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b9cc4-107">Trebali biste očekivati da će te aplikacije tijekom tog vremena doseći ograničen protok.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b9cc4-108">No tijekom večeri i vikenda u regiji servis će biti spreman za obradu znatno većeg volumena zahtjeva iz pozadinske aplikacije.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b9cc4-109">**Performanse migracije**</span><span class="sxs-lookup"><span data-stu-id="b9cc4-109">**Migration performance**</span></span>

<span data-ttu-id="b9cc4-110">Na performanse migracije mogu utjecati mrežna infrastruktura, veličina datoteke, vrijeme migracije te ograničavanje.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="b9cc4-111">Razumijevanje gore navedenog olakšat će vam planiranje i maksimiziranje efikasnosti migracije.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="b9cc4-112">Da biste saznali više, posjetite poveznice u nastavku.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="b9cc4-113">SharePoint Online i brzina ODB migracije</span><span class="sxs-lookup"><span data-stu-id="b9cc4-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="b9cc4-114">Izbjegavanje uskih grla ili blokiranja u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b9cc4-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="b9cc4-115">Preuzimanje i instalacija alata za migraciju sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="b9cc4-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
