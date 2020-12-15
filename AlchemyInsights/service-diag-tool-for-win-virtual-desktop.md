---
title: Alat za dijagnostiku servisa za Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677173"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="357a9-102">Alat za dijagnostiku servisa za Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="357a9-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="357a9-103">Windows Virtual Desktop (WVD) nudi dijagnostički alat koji administratorima omogućuje prepoznavanje pogrešaka putem jednog sučelja.</span><span class="sxs-lookup"><span data-stu-id="357a9-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="357a9-104">Ovaj alat zapisuje informacije vezane uz dijagnostiku ako je netko dodijelio ulogu WVD-a.</span><span class="sxs-lookup"><span data-stu-id="357a9-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="357a9-105">Svaki zapisnik sadrži informacije o ulozi WVD-a uključenih u aktivnost, porukama o pogreškama koje se prikazuju tijekom sesije te informacije o klijentu i korisniku.</span><span class="sxs-lookup"><span data-stu-id="357a9-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="357a9-106">Analitička evidencija Azure može se konfigurirati tako da snimi zapisnik aktivnosti koje je kreirao dijagnostički alat.</span><span class="sxs-lookup"><span data-stu-id="357a9-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="357a9-107">Evo i kako:</span><span class="sxs-lookup"><span data-stu-id="357a9-107">Here's how:</span></span>

1. <span data-ttu-id="357a9-108">Stvorite radni prostor analitike zapisnika uz [portal Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ili [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="357a9-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="357a9-109">[Povežite računala sa sustavom Windows s monitorom Azure](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="357a9-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="357a9-110">Nabavite ID radnog prostora i primarni ključ radnog prostora.</span><span class="sxs-lookup"><span data-stu-id="357a9-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="357a9-111">Čarobnjaku za postavljanje potrebne su te informacije da bi pravilno konfigurirali agenta i da bi se osiguralo da može komunicirati s monitorom Azure.</span><span class="sxs-lookup"><span data-stu-id="357a9-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="357a9-112">[Gurnite dijagnoziranje podataka u radni prostor](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="357a9-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="357a9-113">Dijagnostičke podatke iz servisa WVD možete pritisnuti u analitiku zapisnika za radni prostor.</span><span class="sxs-lookup"><span data-stu-id="357a9-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="357a9-114">[Identificiranje i dijagnosticiranje problema](https://go.microsoft.com/fwlink/?linkid=2128338) koji su interni ili vanjski u odnosu na wvd.</span><span class="sxs-lookup"><span data-stu-id="357a9-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="357a9-115">Dodatne informacije o konfiguriranju alata za dijagnostiku servisa za WVD potražite [u članku Korištenje analitičke analize za značajku dijagnostike](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="357a9-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
