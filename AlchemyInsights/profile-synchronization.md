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
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554325"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="8cb32-102">Kada se moje promjene profila sinkronizirati aplikaciju korisničkog profila sustava SharePoint?</span><span class="sxs-lookup"><span data-stu-id="8cb32-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="8cb32-103">SharePoint Online koristi aktivni imenik uvoz mjerača vremena (AD uvoz) za uvoz korisnike i grupe u aplikaciju korisničkog profila.</span><span class="sxs-lookup"><span data-stu-id="8cb32-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="8cb32-104">Uvoz AD sinkronizira promjene iz SharePoint internetski imenik spremišta aplikaciju korisničkog profila.</span><span class="sxs-lookup"><span data-stu-id="8cb32-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="8cb32-105">Te promjene se obrađuju u skupinama.</span><span class="sxs-lookup"><span data-stu-id="8cb32-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="8cb32-106">Posao mjerača vremena pokreće dok se promjene sinkroniziraju.</span><span class="sxs-lookup"><span data-stu-id="8cb32-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="8cb32-107">Vrijeme pokretanja posla ovisi o broju promjena obraditi.</span><span class="sxs-lookup"><span data-stu-id="8cb32-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="8cb32-108">Velik broj promjena traje dulje.</span><span class="sxs-lookup"><span data-stu-id="8cb32-108">A large number of changes takes longer.</span></span> <span data-ttu-id="8cb32-109">Sporazum o razini usluge (SLA) navodi da Promijeni korisnika u Online imeniku SharePoint odrazit će se u aplikaciju korisničkog profila u 24 sata.</span><span class="sxs-lookup"><span data-stu-id="8cb32-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="8cb32-110">Dodatne informacije o sinkroniziranju korisničkih profila u SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="8cb32-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

