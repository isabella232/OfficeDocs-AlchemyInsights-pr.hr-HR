---
title: Konfiguriranje izuzimanja za Microsoft Defender ATP skeniranja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543677"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="33141-102">Konfiguriranje izuzimanja za Microsoft Defender ATP skeniranja</span><span class="sxs-lookup"><span data-stu-id="33141-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="33141-103">Općenito govoreći, određene datotečne nastavke i mjesta mapa možete izuzeti iz Microsoft Defender ATP skeniranja.</span><span class="sxs-lookup"><span data-stu-id="33141-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="33141-104">Možete konfigurirati i izuzimanja za datoteke otvorene određenim procesima.</span><span class="sxs-lookup"><span data-stu-id="33141-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="33141-105">Dodatne informacije potražite u članku Konfiguriranje i provjera valjanosti [izuzimanja](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) na temelju datotečnog nastavka i mjesta mape te [Konfiguriranje izuzimanja za datoteke otvorene procesima](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="33141-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="33141-106">Da biste konfigurirali **izuzimanja za Windows Server 2016 i 2019**, pogledajte [konfiguriranje Microsoft Defender Antivirus izuzimanja na Windows poslužitelju](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="33141-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="33141-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="33141-107">**Mac**</span></span>

<span data-ttu-id="33141-108">Detalje o podržanim vrstama izuzetka i konfiguraciji popisa izuzimanja za Mac potražite u članku Podržane vrste [izuzetka](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) i Konfiguriranje [popisa izuzimanja](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="33141-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="33141-109">**Napomena** Popise izuzimanja možete provjeriti i pomoću testne datoteke EICAR.</span><span class="sxs-lookup"><span data-stu-id="33141-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="33141-110">Dodatne informacije potražite u članku Provjera [valjanosti popisa izuzimanja pomoću testne datoteke EICAR.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="33141-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="33141-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="33141-111">**Linux**</span></span>

<span data-ttu-id="33141-112">Detalje o podržanim vrstama izuzetka i konfiguraciji popisa [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) izuzimanja za Linux potražite u članku Podržane vrste izuzetka i Konfiguriranje i provjera valjanosti [izuzimanja za Microsoft Defender ATP za Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="33141-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="33141-113">**Napomena** Popise izuzimanja možete provjeriti i pomoću testne datoteke EICAR.</span><span class="sxs-lookup"><span data-stu-id="33141-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="33141-114">Dodatne informacije potražite u članku Provjera [valjanosti popisa izuzimanja pomoću testne datoteke EICAR.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="33141-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 