---
title: Automatsko prijavljivanje u Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676965"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatsko prijavljivanje u Microsoft Edge

Microsoft Edge koristi zadani račun OS-a da bi se automatski prijavljujem u korisnika prema načinu na koji je korisnički uređaj konfiguriran. 

Scenariji svake vrste konfiguracije uređaja i njenog ovisnog korisničkog postupka prijave opisani su u nastavku:

1. **Uređaj je Hybrid/AAD-J**: ta je mogućnost dostupna u sustavu Windows 10, sustavu Windows i pripadajućim poslužiteljskim verzijama. Korisnici se automatski prijave pomoću računa za Azure Active Directory (AD).
2. **Uređaj je spojen na domenu**: ta je mogućnost dostupna u sustavu Windows 10, Windows i pripadajućim poslužiteljskim verzijama. Korisnici s računima domena po zadanom nisu prijavljeni automatski; Da biste omogućili automatsko prijavljivanje za njih, koristite pravilnik **Configureonpremisasaccountautosignin** . Da biste omogućili automatsko prijavljivanje za korisnike s računima za Azure AD, razmotrite hibridno spajanje na njihove uređaje.
3. **Zadani račun OS-a jest Microsoftov račun**: ta je mogućnost dostupna u sustavu Windows 10 RS3 (verzija 1709, izgradnja 10.0.16299) i novije verzije. Scenarij se vjerojatno neće pojaviti na poslovnim uređajima. No ako je zadani račun OS-a Microsoftov račun, Microsoft Edge automatski će se prijaviti korisniku pomoću Microsoftova računa.
 
 
