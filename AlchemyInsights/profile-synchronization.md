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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kada se moj profil promijeni u aplikaciju korisničkog profila sustava SharePoint?

SharePoint Online koristi posao mjerača vremena uvoza Active Directory (Uvoz AD) za uvoz korisnika i grupa u aplikaciju korisničkog profila. 
  
1. Uvoz oglasa sinkronizira promjene iz servisa SharePoint Online Directory Store u aplikaciju korisničkog profila. Te se promjene obrađuju u serijama.
    
2. Posao mjerača vremena izvodi se dok se promjene ne sinkroniziraju.
    
> [!NOTE]
> Vrijeme koje je potrebno za pokretanje posla ovisi o broju promjena u procesu. Veliki broj promjena traje duže. Ugovor o razini usluge (SLA) navodi da će se promjena korisnika u SharePoint Online imeniku odražavati u aplikaciji korisnički profil u roku od 24 sata. 
  
[Dodatne informacije o sinkronizaciji korisničkog profila u sustavu SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

