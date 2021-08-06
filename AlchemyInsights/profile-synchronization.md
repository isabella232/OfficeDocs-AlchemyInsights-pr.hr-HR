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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923636"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kada se promjene profila sinkroniziraju s aplikacijom SharePoint korisničkog profila?

SharePoint Online koristi zadatak mjerača vremena uvoza servisa Active Directory (AD Import) za uvoz korisnika i grupa u aplikaciju korisničkih profila. 
  
1. Ad Import sinkronizira promjene iz trgovine SharePoint online direktorija s aplikacijom korisničkih profila. Te se promjene obrađuju u grupama.
    
2. Zadatak mjerača vremena izvodi se dok se promjene ne sinkroniziraju.
    
> [!NOTE]
> Vrijeme potrebno za pokretanje posla ovisi o broju promjena u postupku. Velik broj promjena traje dulje. U ugovoru o razini usluge (SLA) navodi se da će se promjena na korisnika u direktoriju SharePoint online odražavati u aplikaciji korisničkih profila za 24 sata. 
  
[Dodatne informacije o sinkronizaciji korisničkog profila u web-mjestu SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

