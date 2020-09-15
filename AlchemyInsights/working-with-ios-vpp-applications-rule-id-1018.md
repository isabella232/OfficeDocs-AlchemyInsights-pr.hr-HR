---
title: Rad sa pravilom VPP aplikacija za iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688938"
---
# <a name="working-with-ios-vpp-applications"></a>Rad s aplikacijama sustava iOS VPP

Pročitajte [kako upravljati aplikacijama sustava iOS kupljene putem programa za nabavu u programu Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) da biste saznali više o značajkama, ograničenjima i koracima da biste koristili program Apple Volume Kupnja i podršku za nju u programu Microsoft Intune.
  
 **Česti problemi:** "Korisniku sam dodijelio aplikaciju iOS VPP, ali instalacija nije uspjela."
  
- To se može dogoditi ako se na više davatelja mobilnih uređaja koristi jedan token VPP-a. VPP tokeni iz Apple-a mogu se koristiti samo s jednim davatelja usluga. Ako ste koristili VPP token s više davatelja usluga, morate ponovno prenijeti token na Intune.

- Instalacija može uspjeti i ako ukupan broj instalacija premašuje broj licenci. Da biste pregledali izvješće o korištenju licenci, otvorite stranicu licence za **aplikacije Intune za mobilne aplikacije** \> **App licenses** . Da biste doznali kako povratiti licence koje se koriste, pročitajte [ovaj članak.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
