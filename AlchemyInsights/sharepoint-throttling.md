---
title: Ograničavanje sustava SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931434"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="d1636-102">Ograničavanje sustava SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d1636-102">SharePoint Online throttling</span></span>

<span data-ttu-id="d1636-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="d1636-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d1636-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="d1636-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d1636-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="d1636-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d1636-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="d1636-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d1636-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="d1636-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d1636-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="d1636-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d1636-109">**Ograničavanje sustava SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="d1636-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="d1636-110">SharePoint Online koristi ograničavanje za održavanje optimalnih performansi i pouzdanosti servisa sustava SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="d1636-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="d1636-111">Ograničavanje ograničava broj korisničkih akcija ili istodobnih poziva (po skripti ili kodu) kako bi se spriječilo prekomjerno korištenje resursa.</span><span class="sxs-lookup"><span data-stu-id="d1636-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="d1636-112">Za više informacija, molimo posjetite linkove ispod.</span><span class="sxs-lookup"><span data-stu-id="d1636-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="d1636-113">Izbjegavanje gasija ili blokiranja u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d1636-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="d1636-114">Migracija podataka i ograničavanje SPO-a</span><span class="sxs-lookup"><span data-stu-id="d1636-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="d1636-115">Brzina migracije na SharePoint Online i OneDrive</span><span class="sxs-lookup"><span data-stu-id="d1636-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="d1636-116">Upravljanje ograničavanjem sustava SharePoint Online pomoću eksponencijalnog isključivanja</span><span class="sxs-lookup"><span data-stu-id="d1636-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="d1636-117">Planiranje kapaciteta i testiranje opterećenja sustava SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d1636-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

