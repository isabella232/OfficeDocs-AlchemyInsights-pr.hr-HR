---
title: Problemi s onboarding strojevima
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141320"
---
# <a name="issues-with-onboarding-machines"></a>Problemi s onboarding strojevima

Možda imate problema s onboarding strojevima za MDATP uslugu. Ako možete pristupiti računalu krajnjeg korisnika, slijedite ove korake:

1. Preuzmite dijagnostički alat [za analizu povezivosti klijenta.](https://aka.ms/mdatpanalyzer)
2. Ekstrakt i trčanje MDATPAnalyzer.cmd.
3. Pronađite dijagnostički zapisnik u mapi pod nazivom MDATPClientAnalyzerResult, istu mapu u kojoj se preuzima alat Analizator.
4. Pregledajte datoteku zapisnika, MDATPClientAnalyzer.txt, da biste pronašli probleme s postavkama povezivanja ili postavki internetskog proxyja.