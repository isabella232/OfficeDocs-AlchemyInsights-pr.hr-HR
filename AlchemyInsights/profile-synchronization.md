---
title: Sinkronizacija profila
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801761"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kada se moj profil mijenja u aplikaciju korisničkog profila u sustavu SharePoint?

SharePoint Online koristi posao mjerača vremena uvoza servisa Active Directory (Uvoz oglasa) za uvoz korisnika i grupa u aplikaciju korisničkog profila. 
  
1. Uvoz oglasa sinkronizira promjene iz direktorija imenika sustava SharePoint Online u aplikaciju korisničkog profila. Te se promjene obrađuju u serijama.
    
2. Zadatak mjerača vremena pokrenut će se dok se promjene ne sinkroniziraju.
    
> [!NOTE]
> Vrijeme koje je potrebno pokrenuti posao ovisi o broju promjena u obradi. Veliki broj promjena traje dulje. Ugovor o razini servisa (SLA) navodi da će se promjena korisnika u direktoriju sustava SharePoint Online odraziti u aplikaciji korisnički profil u 24 sata. 
  
[Dodatne informacije o sinkronizaciji korisničkog profila u sustavu SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

