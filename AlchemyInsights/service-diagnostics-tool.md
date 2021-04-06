---
title: Alat za dijagnostiku servisa za virtualnu radnu površinu sustava Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595516"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="f67c4-102">Alat za dijagnostiku servisa za virtualnu radnu površinu sustava Windows</span><span class="sxs-lookup"><span data-stu-id="f67c4-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="f67c4-103">Windows Virtual Desktop (WVD) nudi dijagnostički alat koji administratorima omogućuje prepoznavanje pogrešaka putem jednog sučelja.</span><span class="sxs-lookup"><span data-stu-id="f67c4-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="f67c4-104">Taj alat zapisuje podatke vezane uz dijagnostiku svaki put kada WVD koristi netko kome je dodijeljena WVD uloga.</span><span class="sxs-lookup"><span data-stu-id="f67c4-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="f67c4-105">Svaki zapisnik sadrži informacije o ulozi WVD-a uključenoj u aktivnost, porukama o pogreškama koje se prikazuju tijekom sesije te podacima o klijentu i korisniku.</span><span class="sxs-lookup"><span data-stu-id="f67c4-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="f67c4-106">Analitika zapisnika servisa Azure može se konfigurirati tako da bilježi zapisnik aktivnosti koji je stvorio dijagnostički alat na sljedeći način:</span><span class="sxs-lookup"><span data-stu-id="f67c4-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="f67c4-107">Stvorite radni prostor analitike zapisnika pomoću [portala Azure ili](https://go.microsoft.com/fwlink/?linkid=2129500) [komponente Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="f67c4-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="f67c4-108">[Povežite računala sa sustavom Windows sa servisom Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="f67c4-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="f67c4-109">Nabavite ID radnog prostora i primarni ključ radnog prostora.</span><span class="sxs-lookup"><span data-stu-id="f67c4-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="f67c4-110">Čarobnjaku za postavljanje potrebni su ti podaci da bi agent pravilno konfigurirao i kako bi mogao komunicirati sa servisom Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="f67c4-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="f67c4-111">[Gurnite dijagnostičke podatke u radni prostor](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="f67c4-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="f67c4-112">Dijagnostičke podatke s WVD klijenta možete prenjeti u analitiku zapisnika za radni prostor.</span><span class="sxs-lookup"><span data-stu-id="f67c4-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="f67c4-113">[Prepoznajte i dijagnosticirajte probleme](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) koji su interni ili vanjski u odnosu na WVD.</span><span class="sxs-lookup"><span data-stu-id="f67c4-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="f67c4-114">Dodatne informacije o konfiguraciji alata za dijagnostiku servisa za WVD potražite u članku Korištenje analitike zapisnika za značajku dijagnostike.</span><span class="sxs-lookup"><span data-stu-id="f67c4-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>