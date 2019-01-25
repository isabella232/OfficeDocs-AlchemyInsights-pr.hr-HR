---
title: Rad s iOS VPP aplikacije pravilo Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29461931"
---
# <a name="working-with-ios-vpp-applications"></a>Rad s iOS VPP aplikacija

Čitanje [kako upravljati apps iOS kupili putem glasnoće nabave program s Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) da biste saznali više o značajki, ograničenja i korake da bi koristiti Apple glasnoće nabave Program i podrška za njega u Microsoft Intune. 
  
 **Uobičajene probleme:** "Dodijeljeni app VPP je iOS Moje korisnici, ali instalacija nije uspjela." 
  
- To se može dogoditi ako se koristi jedan token VPP preko višestruke davatelje usluga upravljanja mobilnog uređaja. VPP tokeni iz Apple se može koristiti samo s jednog davatelja. Koristi VPP token s višestruke davatelje usluga, morate ponovo prenesite token Intune.
    
- Instalacija također neće uspeti ako ukupan broj instalacijama prijeći broj licenci. Prikaz izvješća o korištenju licence, idite na **apps Intune Mobile** \> stranici **App licence** . Da biste saznali kako oslobodio licenci koristi pogledajte [Ovaj članak.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

