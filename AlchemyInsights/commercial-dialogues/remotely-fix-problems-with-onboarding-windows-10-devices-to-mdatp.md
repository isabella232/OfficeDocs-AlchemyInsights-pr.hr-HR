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
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="0aa82-102">Daljinsko otklanjanje problema s povezivanjem uređaja sa sustavom Windows 10 u programu Microsoft Defender Napredno zaštita od prijetnje</span><span class="sxs-lookup"><span data-stu-id="0aa82-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="0aa82-103">Ako možete pristupiti udaljenom računalu, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="0aa82-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="0aa82-104">Preuzmite dijagnostički alat za [analizu povezivanja s klijentom](https://go.microsoft.com/fwlink/?linkid=2143466) .</span><span class="sxs-lookup"><span data-stu-id="0aa82-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="0aa82-105">Ekstrakt i trčanje MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="0aa82-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="0aa82-106">Pronađite Dijagnostički zapisnik u mapi Mdatpclientanalyzer (rezultat), koja je ista mapa u kojoj je preuzeta alat za analizu.</span><span class="sxs-lookup"><span data-stu-id="0aa82-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="0aa82-107">Da biste pronašli probleme s povezivanjem ili postavkama internetskog proxyja, pregledajte MDATPClientAnalyzer.txt datoteka zapisnika.</span><span class="sxs-lookup"><span data-stu-id="0aa82-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="0aa82-108">Dodatne informacije potražite u članku [Problemi s uređajima za ukrcavanje](https://go.microsoft.com/fwlink/?linkid=2143634).</span><span class="sxs-lookup"><span data-stu-id="0aa82-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
