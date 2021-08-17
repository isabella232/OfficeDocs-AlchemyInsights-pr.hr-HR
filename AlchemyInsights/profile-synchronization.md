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
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320701"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kada se promjene profila sinkroniziraju s aplikacijom SharePoint korisničkog profila?

SharePoint Online koristi zadatak mjerača vremena uvoza servisa Active Directory (AD Import) za uvoz korisnika i grupa u aplikaciju korisničkih profila. 
  
1. Ad Import sinkronizira promjene iz trgovine SharePoint direktorija u aplikaciju korisničkih profila. Te se promjene obrađuju u grupama.
    
2. Zadatak mjerača vremena izvodi se dok se promjene ne sinkroniziraju.
    
**Napomena**: vrijeme potrebno za pokretanje posla ovisi o broju promjena u postupku. Velik broj promjena traje dulje. U ugovoru o razini servisa (SLA) navodi se da će se promjena na korisnika u mrežnom direktoriju sustava SharePoint odražavati u aplikaciji korisničkog profila za 24 sata. 
  
[Dodatne informacije o sinkronizaciji korisničkog profila na servisu SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

