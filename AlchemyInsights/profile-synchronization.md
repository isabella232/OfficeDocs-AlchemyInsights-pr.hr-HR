---
title: Sinkronizacija profila
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554325"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="45755-102">Kada se moj profil promijeni u aplikaciju korisničkog profila sustava SharePoint?</span><span class="sxs-lookup"><span data-stu-id="45755-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="45755-103">SharePoint Online koristi posao mjerača vremena uvoza Active Directory (Uvoz AD) za uvoz korisnika i grupa u aplikaciju korisničkog profila.</span><span class="sxs-lookup"><span data-stu-id="45755-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="45755-104">Uvoz oglasa sinkronizira promjene iz servisa SharePoint Online Directory Store u aplikaciju korisničkog profila.</span><span class="sxs-lookup"><span data-stu-id="45755-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="45755-105">Te se promjene obrađuju u serijama.</span><span class="sxs-lookup"><span data-stu-id="45755-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="45755-106">Posao mjerača vremena izvodi se dok se promjene ne sinkroniziraju.</span><span class="sxs-lookup"><span data-stu-id="45755-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="45755-107">Vrijeme koje je potrebno za pokretanje posla ovisi o broju promjena u procesu.</span><span class="sxs-lookup"><span data-stu-id="45755-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="45755-108">Veliki broj promjena traje duže.</span><span class="sxs-lookup"><span data-stu-id="45755-108">A large number of changes takes longer.</span></span> <span data-ttu-id="45755-109">Ugovor o razini usluge (SLA) navodi da će se promjena korisnika u SharePoint Online imeniku odražavati u aplikaciji korisnički profil u roku od 24 sata.</span><span class="sxs-lookup"><span data-stu-id="45755-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="45755-110">Dodatne informacije o sinkronizaciji korisničkog profila u sustavu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="45755-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

