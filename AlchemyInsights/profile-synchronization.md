---
title: Sinkronizacija profila
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768105"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="a9bf7-102">Kada se moj profil mijenja u sinkronizaciju sa sharepoint aplikacijom korisničkog profila?</span><span class="sxs-lookup"><span data-stu-id="a9bf7-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="a9bf7-103">SharePoint Online koristi zadatak mjerača vremena uvoza servisa Active Directory (AD Uvoz) za uvoz korisnika i grupa u aplikaciju korisničkog profila.</span><span class="sxs-lookup"><span data-stu-id="a9bf7-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="a9bf7-104">AD uvoz sinkronizira promjene iz spremišta direktorija sustava SharePoint Online u aplikaciju korisničkog profila.</span><span class="sxs-lookup"><span data-stu-id="a9bf7-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="a9bf7-105">Te se promjene obrađuju u serijama.</span><span class="sxs-lookup"><span data-stu-id="a9bf7-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="a9bf7-106">Zadatak mjerača vremena pokreće se dok se promjene ne sinkroniziraju.</span><span class="sxs-lookup"><span data-stu-id="a9bf7-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="a9bf7-107">Vrijeme potrebno za pokretanje posla ovisi o broju promjena koje treba obraditi.</span><span class="sxs-lookup"><span data-stu-id="a9bf7-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="a9bf7-108">Velik broj promjena traje duže.</span><span class="sxs-lookup"><span data-stu-id="a9bf7-108">A large number of changes takes longer.</span></span> <span data-ttu-id="a9bf7-109">Ugovor o razini usluge (SLA) navodi da će se promjena korisnika u imeniku sustava SharePoint Online odraziti u aplikaciji korisničkog profila za 24 sata.</span><span class="sxs-lookup"><span data-stu-id="a9bf7-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="a9bf7-110">Dodatne informacije o sinkronizaciji korisničkog profila u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a9bf7-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

