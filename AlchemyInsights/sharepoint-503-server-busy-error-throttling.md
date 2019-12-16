---
title: Reguliranje sustava SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048608"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="7861d-102">Reguliranje sustava SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7861d-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="7861d-103">Korisnici mogu primiti 503 poslužitelj je zauzet pogreška prilikom pokušaja navigacije na SharePoint ili OneDrive web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="7861d-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="7861d-104">Ta se pogreška može uzrokovati ograničavanjem unutar SharePoint servisa.</span><span class="sxs-lookup"><span data-stu-id="7861d-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="7861d-105">SharePoint Online koristi ograničavanje za održavanje optimalne performanse i pouzdanost usluge SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="7861d-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="7861d-106">Reguliranje ograničava broj korisničkih akcija ili istodobnih poziva (po skripti ili kodu) kako bi se spriječilo prekomjerno korištenje resursa.</span><span class="sxs-lookup"><span data-stu-id="7861d-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="7861d-107">Ako se ograniči, 99% vremena je zbog prilagođenog koda.</span><span class="sxs-lookup"><span data-stu-id="7861d-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="7861d-108">Za više informacija o regulaciji Pogledajte, [Izbjegavajte ograničavanje ili blokiranje u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="7861d-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="7861d-109">Ako smatrate da ova pogreška nije povezana s regulacijom, možete provjeriti postoji li aktivno održavanje koje se pojavljuje na vašem klijentu tako da navigirate do [centra za poruke](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="7861d-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="7861d-110">Konačno, provjerite jeste li posjetili stranicu [zdravstvene usluge](https://portal.office.com/adminportal/home#/servicehealth) kako biste provjerili ima li ikakvih savjetovanja/incidenata koji se možda javljaju.</span><span class="sxs-lookup"><span data-stu-id="7861d-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

