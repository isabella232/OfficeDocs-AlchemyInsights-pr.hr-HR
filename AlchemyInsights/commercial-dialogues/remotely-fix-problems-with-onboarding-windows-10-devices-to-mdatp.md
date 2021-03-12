---
title: Daljinsko otklanjanje problema s povezivanjem uređaja sa sustavom Windows 10 u programu Microsoft Defender Napredno zaštita od prijetnje
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743780"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Daljinsko otklanjanje problema s povezivanjem uređaja sa sustavom Windows 10 u programu Microsoft Defender Napredno zaštita od prijetnje

Ako možete pristupiti udaljenom računalu, slijedite ove korake:

1. Preuzmite dijagnostički alat za [analizu povezivanja s klijentom](https://go.microsoft.com/fwlink/?linkid=2143466) .
2. Ekstrakt i trčanje MDATPAnalyzer. cmd.
3. Pronađite Dijagnostički zapisnik u mapi Mdatpclientanalyzer (rezultat), koja je ista mapa u kojoj je preuzeta alat za analizu.
4. Da biste pronašli probleme s povezivanjem ili postavkama internetskog proxyja, pregledajte MDATPClientAnalyzer.txt datoteka zapisnika.

Dodatne informacije potražite u članku [Problemi s uređajima za ukrcavanje](https://go.microsoft.com/fwlink/?linkid=2143634).
