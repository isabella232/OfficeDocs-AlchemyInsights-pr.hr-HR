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
ms.openlocfilehash: ed3598dc92a7c36c9c9b077db0ab31f63537ef60
ms.sourcegitcommit: 14894a09db1c4101e48ff720d878d1c9f7b1dac8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/16/2019
ms.locfileid: "40065550"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="2caae-102">Reguliranje sustava SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2caae-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="2caae-103">Korisnici mogu primiti 503 poslužitelj je zauzet pogreška prilikom pokušaja navigacije na SharePoint ili OneDrive web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="2caae-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="2caae-104">Ta se pogreška može uzrokovati ograničavanjem unutar SharePoint servisa.</span><span class="sxs-lookup"><span data-stu-id="2caae-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="2caae-105">SharePoint Online koristi ograničavanje za održavanje optimalne performanse i pouzdanost usluge SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="2caae-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="2caae-106">Reguliranje ograničava broj korisničkih akcija ili istodobnih poziva (po skripti ili kodu) kako bi se spriječilo prekomjerno korištenje resursa.</span><span class="sxs-lookup"><span data-stu-id="2caae-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="2caae-107">Za više informacija o regulaciji Pogledajte, [Izbjegavajte ograničavanje ili blokiranje u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="2caae-107">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="2caae-108">Ako smatrate da ova pogreška nije povezana s regulacijom, možete provjeriti postoji li aktivno održavanje koje se pojavljuje na vašem klijentu tako da navigirate do [centra za poruke](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="2caae-108">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="2caae-109">Konačno, provjerite jeste li posjetili stranicu [zdravstvene usluge](https://portal.office.com/adminportal/home#/servicehealth) kako biste provjerili ima li ikakvih savjetovanja/incidenata koji se možda javljaju.</span><span class="sxs-lookup"><span data-stu-id="2caae-109">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

