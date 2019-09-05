---
title: Online Reguliranje SharePoint
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751880"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="5cf11-102">Online Reguliranje SharePoint</span><span class="sxs-lookup"><span data-stu-id="5cf11-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="5cf11-103">Korisnici mogu primati na 503 poslužitelj je zauzet pogreška prilikom pokušaja idite do mjesta SharePoint ili OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5cf11-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="5cf11-104">Ova pogreška može uzrok Reguliranje unutar usluge SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5cf11-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="5cf11-105">SharePoint Online koristi Reguliranje za održavanje optimalnih performansi i pouzdanosti usluge SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="5cf11-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5cf11-106">Reguliranje ograničava broj akcije korisnika ili Istodobni poziva (po skripta ili kod) spriječiti Prekomjerno korištenje resursa.</span><span class="sxs-lookup"><span data-stu-id="5cf11-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="5cf11-107">Ako ste dobili ograničio vrijeme, 99% vrijeme je radi prilagođenog koda.</span><span class="sxs-lookup"><span data-stu-id="5cf11-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="5cf11-108">Dodatne informacije o Reguliranje pogledajte [Avoid dobivanju ograničio vrijeme ili blokiran u SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="5cf11-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="5cf11-109">Ako mislite da se ova pogreška nepovezane reguliranje, možete provjeriti ako postoji aktivni održavanja pojavljivanja na vašem klijentske odlaskom na [poruku centar](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="5cf11-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="5cf11-110">Konačno, provjerite posjetite stranicu [Servisa stanja sustava](https://portal.office.com/adminportal/home#/servicehealth) da biste provjerili sve advisories/incidenata koji možda pojavljivanja.</span><span class="sxs-lookup"><span data-stu-id="5cf11-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

