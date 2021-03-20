---
title: Problemi s uređajima za ukrcavanje u Microsoft Defender za krajnje točke
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
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901559"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="95bc6-102">Problemi s uređajima za ukrcavanje u Microsoft Defender za krajnje točke</span><span class="sxs-lookup"><span data-stu-id="95bc6-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="95bc6-103">Možda imate problema s uređajima za ukrcavanje na servisu MDE.</span><span class="sxs-lookup"><span data-stu-id="95bc6-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="95bc6-104">Ako možete pristupiti stroju krajnjeg korisnika, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="95bc6-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="95bc6-105">Preuzmite najnoviju verziju pretpregleda dijagnostičkog alata [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="95bc6-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="95bc6-106">Desnom tipkom miša kliknite **Mdeclientanalyzer. cmd** , a zatim odaberite "Pokreni kao administrator".</span><span class="sxs-lookup"><span data-stu-id="95bc6-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="95bc6-107">Slijedite sve smjernice predložene u **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="95bc6-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="95bc6-108">Da biste dobili više verbose zapisnika, pregledajte kreirani podmapu pod nazivom **Mdeclientanalyzerresult**.</span><span class="sxs-lookup"><span data-stu-id="95bc6-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="95bc6-109">Ako je potrebno dodatno navođenje, obratite se [Microsoftovoj branitelju za podršku za krajnje točke](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) i navedite MDEClientAnalyzerResult.zip datoteku za analizu.</span><span class="sxs-lookup"><span data-stu-id="95bc6-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
