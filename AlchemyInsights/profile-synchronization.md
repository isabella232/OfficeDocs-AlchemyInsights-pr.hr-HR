---
title: Sinkronizacije profila
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371976"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="6b50e-102">Kada se moje promjene profila sinkronizirati aplikaciju korisničkog profila sustava SharePoint?</span><span class="sxs-lookup"><span data-stu-id="6b50e-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="6b50e-103">SharePoint Online koristi aktivni imenik uvoz mjerača vremena (AD uvoz) za uvoz korisnike i grupe u aplikaciju korisničkog profila.</span><span class="sxs-lookup"><span data-stu-id="6b50e-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="6b50e-104">Uvoz AD sinkronizira promjene iz SharePoint internetski imenik spremišta aplikaciju korisničkog profila.</span><span class="sxs-lookup"><span data-stu-id="6b50e-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="6b50e-105">Te promjene se obrađuju u skupinama.</span><span class="sxs-lookup"><span data-stu-id="6b50e-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="6b50e-106">Posao mjerača vremena pokreće dok se promjene sinkroniziraju.</span><span class="sxs-lookup"><span data-stu-id="6b50e-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="6b50e-107">Vrijeme pokretanja posla ovisi o broju promjena obraditi.</span><span class="sxs-lookup"><span data-stu-id="6b50e-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="6b50e-108">Velik broj promjena traje dulje.</span><span class="sxs-lookup"><span data-stu-id="6b50e-108">A large number of changes takes longer.</span></span> <span data-ttu-id="6b50e-109">Sporazum o razini usluge (SLA) navodi da Promijeni korisnika u Online imeniku SharePoint odrazit će se u aplikaciju korisničkog profila u 24 sata.</span><span class="sxs-lookup"><span data-stu-id="6b50e-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="6b50e-110">Dodatne informacije o sinkroniziranju korisničkih profila u SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6b50e-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

