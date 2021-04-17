---
title: MC210173 – obustava značajke za stvaranje novog prilagođenog obrasca u programu SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831798"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="eca66-102">MC210173 – obustava značajke za stvaranje novog prilagođenog obrasca u programu SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="eca66-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="eca66-103">Otkrili smo problem koji utječe na funkcionalnost programa SharePoint Designer za [stvaranje prilagođenih obrazaca](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) u usluzi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="eca66-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="eca66-104">Nakon pažljivog razmatranja, utvrdili smo da ne postoji nijedno poznato rješenje tog problema te smo stoga odlučili da onemogućimo značajku za stvaranje prilagođenih obrazaca. Značajka je prestala biti dostupna u 3:00 (UTC) u subotu, 25. travnja 2020.</span><span class="sxs-lookup"><span data-stu-id="eca66-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="eca66-105">Ta promjena ne utječe na mogućnost uređivanja prethodno stvorenih obrazaca ili drugih postojećih značajki u programu SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="eca66-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="eca66-106">Nakon što je promjena stupila na snagu, korisnici su mogli dobiti pogrešku: „Spremanje promjena popisa na poslužitelju nije uspjelo“ prilikom stvaranja novih obrazaca.</span><span class="sxs-lookup"><span data-stu-id="eca66-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="eca66-107">Korisnici koji su prethodno iskoristili mogućnost programa SharePoint Designer za stvaranje prilagođenih obrazaca od sada u tu svrhu mogu koristiti [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).</span><span class="sxs-lookup"><span data-stu-id="eca66-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="eca66-108">PowerApps je jednostavan i moćan alat koji korisnicima modernog sučelja usluge SharePoint Online omogućuje stvaranje i uređivanje prilagođenih obrazaca za popise programa SharePoint i biblioteke dokumenata izravno u prozoru preglednika.</span><span class="sxs-lookup"><span data-stu-id="eca66-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="eca66-109">PowerApps ne zahtijeva tradicionalno znanje kodiranja ni dodatna preuzimanja aplikacija, kao što je InfoPath.</span><span class="sxs-lookup"><span data-stu-id="eca66-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="eca66-110">**Napomena**: korisnici klasičnog sučelja usluge SharePoint Online moraju privremeno prijeći na moderno sučelje kako bi pristupali aplikacijama PowerApps i koristili ih. Međutim, svi prilagođeni obrasci stvoreni u aplikaciji PowerApps dostupni su korisnicima klasičnog sučelja usluge SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="eca66-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
