---
title: Rad s iOS VPP aplikacije pravilo Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364836"
---
# <a name="working-with-ios-vpp-applications"></a>Rad s iOS VPP aplikacija

Čitanje [kako upravljati apps iOS kupili putem glasnoće nabave program s Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) da biste saznali više o značajki, ograničenja i korake da bi koristiti Apple glasnoće nabave Program i podrška za njega u Microsoft Intune.
  
 **Uobičajene probleme:** "Dodijeljeni app VPP je iOS Moje korisnici, ali instalacija nije uspjela."
  
- To se može dogoditi ako se koristi jedan token VPP preko višestruke davatelje usluga upravljanja mobilnog uređaja. VPP tokeni iz Apple se može koristiti samo s jednog davatelja. Koristi VPP token s višestruke davatelje usluga, morate ponovo prenesite token Intune.

- Instalacija također neće uspeti ako ukupan broj instalacijama prijeći broj licenci. Prikaz izvješća o korištenju licence, idite na **apps Intune Mobile** \> stranici **App licence** . Da biste saznali kako oslobodio licenci koristi pogledajte [Ovaj članak.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
