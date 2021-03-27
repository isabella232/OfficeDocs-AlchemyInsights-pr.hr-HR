---
title: Automatska prijava u Microsoft Edge
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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398721"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatska prijava u Microsoft Edge

Microsoft Edge koristi zadani račun operacijskog sustava za automatsku prijavu korisnika u skladu s konfiguracijom korisnikova uređaja. 

Scenariji svake vrste konfiguracije uređaja i postupka prijave zavisnog korisnika opisani su u nastavku:

- **Uređaj je hibridni/AAD-J:** ta je mogućnost dostupna u sustavima Windows 10, sustavu Windows i odgovarajućim verzijama poslužitelja. Korisnici se automatski prijave pomoću računa servisa Azure Active Directory (AD).
- **Uređaj je pridružen domeni: ta** je mogućnost dostupna u sustavima Windows 10, sustavu Windows nižu razinu i odgovarajućim verzijama poslužitelja. Korisnici s računima domene po zadanom se ne prijave automatski; da biste omogućili automatsku prijavu za njih, koristite **pravilnik ConfigureOnPremisesAccountAutoSignIn.** Da biste korisnicima omogućili automatsku prijavu s računima za Azure AD, razmislite o hibridnom pridruživanju svojim uređajima.
- **Zadani je račun** operacijskog sustava Microsoftov račun: ta je mogućnost dostupna u sustavu Windows 10 RS3 (verzija 1709, međuverzija 10.0.16299) i novijim verzijama. Scenarij nije vjerojatno da će se pojaviti na poslovnim uređajima. No ako je zadani račun za OS Microsoftov račun, Microsoft Edge će se automatski prijaviti korisniku pomoću Microsoftova računa.
 
 
