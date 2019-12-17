---
title: Problemi s performansama – SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068386"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="809d0-102">SharePoint ili OneDrive sporo, nedostupno ili nije dostupno za više korisnika</span><span class="sxs-lookup"><span data-stu-id="809d0-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="809d0-103">SharePoint ili OneDrive može biti spor, nedostupan ili nedostupan ili može prikazati servis nedostupan ili 503 pogreške, iz nekoliko razloga:</span><span class="sxs-lookup"><span data-stu-id="809d0-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="809d0-104">Ako je web-mjesto sustava SharePoint ili OneDrive sporo ili odgođeno za više korisnika, možda postoji problem s privremenim servisom u kojem korisnici doživljavaju povremene odgode ili pogreške u navigaciji pri pristupu SharePoint web-lokacijama ili sadržaju servisa OneDrive.</span><span class="sxs-lookup"><span data-stu-id="809d0-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="809d0-105">Provjerite je li vaša tvrtka ili ustanova utjecala na [nadzornu ploču za zdravlje servisa](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) .</span><span class="sxs-lookup"><span data-stu-id="809d0-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="809d0-106">Korisnici mogu primiti *503 poslužitelj je zauzet* pogreška prilikom pokušaja navigacije na SharePoint ili OneDrive web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="809d0-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="809d0-107">Ta se pogreška može uzrokovati ograničavanjem unutar SharePoint servisa.</span><span class="sxs-lookup"><span data-stu-id="809d0-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="809d0-108">SharePoint Online koristi ograničavanje za održavanje optimalne performanse i pouzdanost usluge SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="809d0-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="809d0-109">Reguliranje ograničava broj korisničkih akcija ili istodobnih poziva (po skripti ili kodu) kako bi se spriječilo prekomjerno korištenje resursa.</span><span class="sxs-lookup"><span data-stu-id="809d0-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="809d0-110">Za više informacija o regulaciji Pogledajte, [Izbjegavajte ograničavanje ili blokiranje u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="809d0-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="809d0-111">Ako osjetite spore performanse s **klasičnim** ili **modernim** SharePoint web-mjestom ili stranicom, upotrijebite [dijagnostički alat stranice](https://aka.ms/perftool) za analizu stranica.</span><span class="sxs-lookup"><span data-stu-id="809d0-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="809d0-112">Ako i dalje doživite opću sporu izvedbu, pregledajte resurse na dnu ovog članka: [Uvod u podešavanje performansi za SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="809d0-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  