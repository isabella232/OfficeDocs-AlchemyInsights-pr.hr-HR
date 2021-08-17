---
title: Rad s ID-om pravila VPP aplikacija sustava iOS 1018
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
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083006"
---
# <a name="working-with-ios-vpp-applications"></a>Rad s VPP aplikacijama za iOS

Pročitajte [članak Upravljanje aplikacijama sustava iOS](https://docs.microsoft.com/intune/vpp-apps-ios) kupljenima putem programa za količinu kupnje pomoću programa Microsoft Intune da biste saznali više o značajkama, ograničenjima i koracima za korištenje appleskog programa za količinu kupnje i podrške za njega u Microsoft Intune.
  
 **Uobičajeni problemi:** "Korisnicima sam dodijelio VPP aplikaciju za iOS, ali instalacija nije uspjela."
  
- To se može dogoditi ako se jedan VPP token koristi u više davatelja usluga upravljanja mobilnim uređajima. VPP tokeni tvrtke Apple mogu se koristiti samo s jednim davateljem. Ako ste VPP token koristili s više davatelja, morate ponovno prenijeti token u Intune.

- Instalacija može uspjeti i ako ukupan broj instalacija premašuje broj licenci. Da biste pogledali izvješće o korištenju licenci, idite na stranicu Licence aplikacija **Aplikacije Intune Mobile.** \>  Upute za povrat licenci u upotrebi potražite u [ovom članku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
