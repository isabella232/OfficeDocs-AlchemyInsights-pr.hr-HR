---
title: Ograničavanje sustava SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773839"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="1ecfd-102">Ograničavanje sustava SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="1ecfd-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="1ecfd-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="1ecfd-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="1ecfd-104">**Pogreška sustava 503 je zauzeta**</span><span class="sxs-lookup"><span data-stu-id="1ecfd-104">**503 server is busy error**</span></span>

<span data-ttu-id="1ecfd-105">Kada pokušate prijeći na SharePoint ili web-mjesta servisa OneDrive, korisnici mogu primiti 503 poslužitelj je zauzet.</span><span class="sxs-lookup"><span data-stu-id="1ecfd-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="1ecfd-106">Ovu pogrešku može prouzročiti ograničavanje unutar servisa sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1ecfd-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="1ecfd-107">SharePoint Online koristi ograničavanje za održavanje optimalnih performansi i pouzdanosti servisa SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1ecfd-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="1ecfd-108">Ograničavanjem se ograničava broj korisničkih radnji ili istodobnih poziva (skriptom ili kodom) radi sprječavanja prekomjernog korištenja resursa.</span><span class="sxs-lookup"><span data-stu-id="1ecfd-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="1ecfd-109">Dodatne informacije o [ograničavanju potražite u članku izbjegavanje ograničenja ili blokiranja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="1ecfd-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="1ecfd-110">Ako smatrate da ta pogreška nije vezana uz ograničavanje, možete provjeriti postoji li aktivno održavanje koje se nalazi na vašem zakupcu tako da dođete do [centra za poruke](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="1ecfd-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="1ecfd-111">Konačno, provjerite jeste li na stranici [zdravlje servisa](https://portal.office.com/adminportal/home#/servicehealth) provjerili ima li nekih savjeta/incidenata koji se mogu pojavljivati.</span><span class="sxs-lookup"><span data-stu-id="1ecfd-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

