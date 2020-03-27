---
title: Trajno brisanje web-mjesta u sustavu SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955132"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="91068-102">Trajno brisanje web-mjesta u sustavu SharePoint</span><span class="sxs-lookup"><span data-stu-id="91068-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="91068-103">Da biste ponovno upotrijebili URL s izbrisanog web-mjesta (za ponovno stvaranje web-mjesta) ili da biste trajno izbrisali web-mjesto jer se više ne koristi, možete koristiti **Trajno brisanje** iz novog centra za administratore sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="91068-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="91068-104">Idite na [Stranica za izbrisana web-mjesta novog centra za administratore sustava SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) i prijavite se računom koji ima administratorske dozvole za vašu tvrtku ili ustanovu.</span><span class="sxs-lookup"><span data-stu-id="91068-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="91068-105">U lijevom stupcu odaberite web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="91068-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="91068-106">Kliknite **Trajno brisanje**.</span><span class="sxs-lookup"><span data-stu-id="91068-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="91068-107">**Napomena**: web-mjesta povezana s grupom ne mogu se trajno izbrisati iz novog centra za administratore sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="91068-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="91068-108">[Uklanjanje-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) će se morati koristiti umjesto toga.</span><span class="sxs-lookup"><span data-stu-id="91068-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="91068-109">Dodatne informacije potražite u članku [Trajno brisanje web-mjesta](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="91068-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
