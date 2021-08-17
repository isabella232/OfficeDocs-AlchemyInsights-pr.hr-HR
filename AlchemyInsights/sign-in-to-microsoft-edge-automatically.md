---
title: Automatska Microsoft Edge prijava
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
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050686"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatska Microsoft Edge prijava

Microsoft Edge koristi zadani račun operacijskog sustava za automatsku prijavu korisnika u skladu s konfiguracijom korisnikova uređaja. 

Scenariji svake vrste konfiguracije uređaja i postupka prijave zavisnog korisnika opisani su u nastavku:

- **Uređaj je hibridni/AAD-J:** ta je mogućnost dostupna na Windows 10, na razini Windows i odgovarajućim verzijama poslužitelja. Korisnici se automatski prijave pomoću svojih Azure Active Directory (AD)računa.
- **Uređaj je pridružen domeni:** ta je mogućnost dostupna na Windows 10, na razini Windows i odgovarajućim verzijama poslužitelja. Korisnici s računima domene po zadanom se ne prijave automatski; da biste omogućili automatsku prijavu za njih, koristite **pravilnik ConfigureOnPremisesAccountAutoSignIn.** Da biste korisnicima omogućili automatsku prijavu s računima za Azure AD, razmislite o hibridnom pridruživanju svojim uređajima.
- **Zadani je račun operacijskog** sustava Microsoftov račun: ta je mogućnost dostupna u sustavu WINDOWS 10 RS3 (verzija 1709, međuverzija 10.0.16299) i novijim verzijama. Scenarij nije vjerojatno da će se pojaviti na poslovnim uređajima. No ako je zadani račun operacijskog sustava Microsoftov račun, Microsoft Edge će se automatski prijaviti korisniku pomoću Microsoftova računa.
 
 
