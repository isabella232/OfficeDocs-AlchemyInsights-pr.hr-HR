---
title: Ograničavanje sustava SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958710"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="805ca-102">Ograničavanje sustava SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="805ca-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="805ca-103">**Važno**: Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i onedrive ostanu vrlo dostupne – dodatne informacije [potražite u članku Prilagodbe privremenih značajki sustava SharePoint Online.](https://aka.ms/ODSPAdjustments)</span><span class="sxs-lookup"><span data-stu-id="805ca-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="805ca-104">**503 poslužitelj je zauzet greška**</span><span class="sxs-lookup"><span data-stu-id="805ca-104">**503 server is busy error**</span></span>

<span data-ttu-id="805ca-105">Korisnici mogu primiti 503 poslužitelj je zauzet greška prilikom pokušaja navigacije do SharePoint ili OneDrive web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="805ca-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="805ca-106">Ta je pogreška moguće uzrokovati ograničavanjem unutar servisa sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="805ca-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="805ca-107">SharePoint Online koristi ograničavanje za održavanje optimalnih performansi i pouzdanosti servisa sustava SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="805ca-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="805ca-108">Ograničavanje ograničava broj korisničkih akcija ili istodobnih poziva (po skripti ili kodu) kako bi se spriječilo prekomjerno korištenje resursa.</span><span class="sxs-lookup"><span data-stu-id="805ca-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="805ca-109">Dodatne informacije o regulaciji potražite u odjeljku [Izbjegavanje ograničavanja ili blokiranja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="805ca-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="805ca-110">Ako smatrate da ta pogreška nije povezana s ograničavanjem, možete provjeriti postoji li aktivno održavanje na vašem klijentu tako da odete do [centra za poruke](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="805ca-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="805ca-111">Naposljetku, provjerite da posjetite stranicu [Zdravlje servisa](https://portal.office.com/adminportal/home#/servicehealth) da biste provjerili ima li savjeta/incidenata koji se mogu pojaviti.</span><span class="sxs-lookup"><span data-stu-id="805ca-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

