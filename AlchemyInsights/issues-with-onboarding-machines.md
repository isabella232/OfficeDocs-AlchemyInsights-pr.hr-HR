---
title: Problemi s uređajima za ukrcavanje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676874"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="09fd2-102">Problemi s uređajima za ukrcavanje</span><span class="sxs-lookup"><span data-stu-id="09fd2-102">Issues with onboarding machines</span></span>

<span data-ttu-id="09fd2-103">Možda imate problema s uređajima za ukrcavanje na servisu MDATP.</span><span class="sxs-lookup"><span data-stu-id="09fd2-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="09fd2-104">Ako možete pristupiti stroju krajnjeg korisnika, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="09fd2-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="09fd2-105">Preuzmite dijagnostički alat za [analizu povezivanja s klijentom](https://aka.ms/mdatpanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="09fd2-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="09fd2-106">Ekstrakt i trčanje MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="09fd2-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="09fd2-107">Pronađite Dijagnostički zapisnik u mapi Mdatpclientanalyzer, istoj mapi u kojoj je preuzeta alat za analizu.</span><span class="sxs-lookup"><span data-stu-id="09fd2-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="09fd2-108">Pregledajte datoteku zapisnika, MDATPClientAnalyzer.txt i potražite probleme s postavkama internetske veze.</span><span class="sxs-lookup"><span data-stu-id="09fd2-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>