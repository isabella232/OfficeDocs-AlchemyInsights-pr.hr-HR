---
title: Daljinski rješavanje problema s Windows 10 uređajima s programom Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034026"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Daljinski rješavanje problema s Windows 10 uređajima s programom Microsoft Defender Advanced Threat Protection

Ako možete pristupiti udaljenom računalu, slijedite ove korake:

1. Preuzmite [dijagnostički alat za analizu klijentske](https://go.microsoft.com/fwlink/?linkid=2143466) povezivosti.
2. Izdvojite i pokrenite MDATPAnalyzer.cmd.
3. Pronađite dijagnostički zapisnik u mapi MDATPClientAnalyzerResult, koja je ista mapa u kojoj je alat Za analizu preuzet.
4. Da biste pronašli probleme s povezivanjem ili postavkama internetskog proxyja, pregledajte datoteku zapisnika MDATPClientAnalyzer.txt.

Dodatne informacije potražite u članku [Problemi s uređajem za unošenje.](https://go.microsoft.com/fwlink/?linkid=2143634)
