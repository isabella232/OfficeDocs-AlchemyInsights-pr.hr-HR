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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kada se moj profil mijenja u sinkronizaciju sa sharepoint aplikacijom korisničkog profila?

SharePoint Online koristi zadatak mjerača vremena uvoza servisa Active Directory (AD Uvoz) za uvoz korisnika i grupa u aplikaciju korisničkog profila. 
  
1. AD uvoz sinkronizira promjene iz spremišta direktorija sustava SharePoint Online u aplikaciju korisničkog profila. Te se promjene obrađuju u serijama.
    
2. Zadatak mjerača vremena pokreće se dok se promjene ne sinkroniziraju.
    
> [!NOTE]
> Vrijeme potrebno za pokretanje posla ovisi o broju promjena koje treba obraditi. Velik broj promjena traje duže. Ugovor o razini usluge (SLA) navodi da će se promjena korisnika u imeniku sustava SharePoint Online odraziti u aplikaciji korisničkog profila za 24 sata. 
  
[Dodatne informacije o sinkronizaciji korisničkog profila u sustavu SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

