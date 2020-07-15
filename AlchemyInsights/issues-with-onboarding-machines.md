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
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="fe859-102">Problemi s onboarding strojevima</span><span class="sxs-lookup"><span data-stu-id="fe859-102">Issues with onboarding machines</span></span>

<span data-ttu-id="fe859-103">Možda imate problema s onboarding strojevima za MDATP uslugu.</span><span class="sxs-lookup"><span data-stu-id="fe859-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="fe859-104">Ako možete pristupiti računalu krajnjeg korisnika, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="fe859-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="fe859-105">Preuzmite dijagnostički alat [za analizu povezivosti klijenta.](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="fe859-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="fe859-106">Ekstrakt i trčanje MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="fe859-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="fe859-107">Pronađite dijagnostički zapisnik u mapi pod nazivom MDATPClientAnalyzerResult, istu mapu u kojoj se preuzima alat Analizator.</span><span class="sxs-lookup"><span data-stu-id="fe859-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="fe859-108">Pregledajte datoteku zapisnika, MDATPClientAnalyzer.txt, da biste pronašli probleme s postavkama povezivanja ili postavki internetskog proxyja.</span><span class="sxs-lookup"><span data-stu-id="fe859-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>