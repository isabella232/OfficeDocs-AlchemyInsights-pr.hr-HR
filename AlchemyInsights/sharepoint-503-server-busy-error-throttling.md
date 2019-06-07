---
title: Online Reguliranje SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761251"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="16d63-102">Online Reguliranje SharePoint</span><span class="sxs-lookup"><span data-stu-id="16d63-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="16d63-103">Korisnici mogu primati na 503 poslužitelj je zauzet pogreška prilikom pokušaja idite do mjesta SharePoint ili OneDrive.</span><span class="sxs-lookup"><span data-stu-id="16d63-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="16d63-104">Ova pogreška može uzrok Reguliranje unutar usluge SharePoint.</span><span class="sxs-lookup"><span data-stu-id="16d63-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="16d63-105">SharePoint Online koristi Reguliranje za održavanje optimalnih performansi i pouzdanosti usluge SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="16d63-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="16d63-106">Reguliranje ograničava broj akcije korisnika ili Istodobni poziva (po skripta ili kod) spriječiti Prekomjerno korištenje resursa.</span><span class="sxs-lookup"><span data-stu-id="16d63-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="16d63-107">Ako ste dobili ograničio vrijeme, 99% vrijeme je radi prilagođenog koda.</span><span class="sxs-lookup"><span data-stu-id="16d63-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="16d63-108">Dodatne informacije o Reguliranje pogledajte [Avoid dobivanju ograničio vrijeme ili blokiran u SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="16d63-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="16d63-109">Ako mislite da se ova pogreška nepovezane reguliranje, možete provjeriti ako postoji aktivni održavanja pojavljivanja na vašem klijentske odlaskom na [poruku centar](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="16d63-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="16d63-110">Konačno, provjerite posjetite stranicu [Servisa stanja sustava](https://portal.office.com/adminportal/home#/servicehealth) da biste provjerili sve advisories/incidenata koji možda pojavljivanja.</span><span class="sxs-lookup"><span data-stu-id="16d63-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

