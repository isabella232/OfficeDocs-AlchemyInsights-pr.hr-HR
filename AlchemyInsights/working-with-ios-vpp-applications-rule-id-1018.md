---
title: Rad s ID-om pravila za aplikacije za iOS VPP 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719949"
---
# <a name="working-with-ios-vpp-applications"></a>Rad s vpp aplikacijama za iOS

Pročitajte [kako upravljati aplikacijama sustava iOS kupljenima putem programa za kupnju jedinice pomoću](https://docs.microsoft.com/intune/vpp-apps-ios) servisa Microsoft Intune da biste saznali više o značajkama, ograničenjima i koracima za korištenje Appleovog programa za kupnju glasnoće i podrške za njega u programu Microsoft Intune.
  
 **Uobičajeni problemi:** "Korisnicima sam dodijelio iOS VPP aplikaciju, ali instalacija nije uspjela."
  
- To se može dogoditi ako se jedan VPP token koristi u više davatelja usluga upravljanja mobilnim uređajima. VPP tokeni tvrtke Apple smiju se koristiti samo s jednim davateljem usluga. Ako ste koristili VPP token s više davatelja usluga, morate ga ponovno prenijeti na Intune.

- Instalacija također može uspjeti ako ukupan broj instalacija premašuje broj licenci. Da biste pregledali izvješće o korištenju za licence, idite na stranicu Licence **aplikacije Intune za mobilne** \> **aplikacije.** Da biste saznali kako povratiti licence koje se koriste, pogledajte [ovaj članak.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
