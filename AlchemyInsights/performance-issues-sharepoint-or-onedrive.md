---
title: Problemi s performansama – SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771893"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="07e5d-102">SharePoint ili OneDrive spori, nedostupni ili nedostupni za više korisnika</span><span class="sxs-lookup"><span data-stu-id="07e5d-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="07e5d-103">SharePoint ili OneDrive mogu biti spori, nedostupni ili nedostupni ili mogu prikazati servis nedostupni ili 503 pogrešaka, iz nekoliko razloga:</span><span class="sxs-lookup"><span data-stu-id="07e5d-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="07e5d-104">Ako je web-mjesto sustava SharePoint ili OneDrive sporo ili odgođeno za više korisnika, možda postoji privremeni problem s servisom u kojem korisnici mogu doživjeti povremeni kašnjenje ili pogreške prilikom navigacije prilikom pristupanja web-mjestima sustava SharePoint ili sadržaju servisa OneDrive.</span><span class="sxs-lookup"><span data-stu-id="07e5d-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="07e5d-105">Provjerite je li vaša tvrtka ili ustanova utjecala na [nadzornu ploču zdravstvenog stanja servisa](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) .</span><span class="sxs-lookup"><span data-stu-id="07e5d-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="07e5d-106">Kada pokušate prijeći na SharePoint ili web-mjesta servisa OneDrive, korisnici mogu primiti *503 poslužitelj je zauzet* .</span><span class="sxs-lookup"><span data-stu-id="07e5d-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="07e5d-107">Ovu pogrešku može prouzročiti ograničavanje unutar servisa sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="07e5d-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="07e5d-108">SharePoint Online koristi ograničavanje za održavanje optimalnih performansi i pouzdanosti servisa SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="07e5d-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="07e5d-109">Ograničavanjem se ograničava broj korisničkih radnji ili istodobnih poziva (skriptom ili kodom) radi sprječavanja prekomjernog korištenja resursa.</span><span class="sxs-lookup"><span data-stu-id="07e5d-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="07e5d-110">Dodatne informacije o [ograničavanju potražite u članku izbjegavanje ograničenja ili blokiranja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="07e5d-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="07e5d-111">Ako osjetite spore performanse uz **klasično** ili **moderno** web-mjesto sustava SharePoint ili stranicu, upotrijebite [dijagnostički alat za stranicu](https://aka.ms/perftool) da biste analizirali stranice.</span><span class="sxs-lookup"><span data-stu-id="07e5d-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="07e5d-112">Ako i dalje imate općenite spore performanse, pregledajte resurse pri dnu ovog članka: [Uvod u tuning performansi za SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="07e5d-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  