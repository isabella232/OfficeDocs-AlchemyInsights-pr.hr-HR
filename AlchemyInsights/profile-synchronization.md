---
title: Sinkronizacije profila
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29462174"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="5a090-102">Kada se moje promjene profila sinkronizirati aplikaciju korisničkog profila sustava SharePoint?</span><span class="sxs-lookup"><span data-stu-id="5a090-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="5a090-103">SharePoint Online koristi aktivni imenik uvoz mjerača vremena (AD uvoz) za uvoz korisnike i grupe u aplikaciju korisničkog profila.</span><span class="sxs-lookup"><span data-stu-id="5a090-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="5a090-p101">Uvoz AD sinkronizira promjene iz SharePoint internetski imenik spremišta aplikaciju korisničkog profila. Te promjene se obrađuju u skupinama.</span><span class="sxs-lookup"><span data-stu-id="5a090-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="5a090-106">Posao mjerača vremena pokreće dok se promjene sinkroniziraju.</span><span class="sxs-lookup"><span data-stu-id="5a090-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="5a090-p102">Vrijeme pokretanja posla ovisi o broju promjena obraditi. Velik broj promjena traje dulje. Sporazum o razini usluge (SLA) navodi da Promijeni korisnika u Online imeniku SharePoint odrazit će se u aplikaciju korisničkog profila u 24 sata.</span><span class="sxs-lookup"><span data-stu-id="5a090-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="5a090-110">Dodatne informacije o sinkroniziranju korisničkih profila u SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5a090-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

