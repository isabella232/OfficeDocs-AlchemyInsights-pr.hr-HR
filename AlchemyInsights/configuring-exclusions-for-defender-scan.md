---
title: Konfiguriranje isključenja za Microsoft Defender ATP Scan
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713326"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="bcd40-102">Konfiguriranje isključenja za Microsoft Defender ATP Scan</span><span class="sxs-lookup"><span data-stu-id="bcd40-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="bcd40-103">Općenito možete isključiti određene ekstenzije datoteka i lokacije mapa iz programa Microsoft Defender ATP skeniranja.</span><span class="sxs-lookup"><span data-stu-id="bcd40-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="bcd40-104">Možete i konfigurirati izuzeće za datoteke koje se otvaraju u određenim procesima.</span><span class="sxs-lookup"><span data-stu-id="bcd40-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="bcd40-105">Dodatne informacije potražite u članku [Konfiguriranje i provjera valjanosti izuzeća na temelju proširenja datoteka i mjesta mape](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) te [Konfiguriranje isključenja za datoteke koje se otvaraju pomoću procesa](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="bcd40-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="bcd40-106">Da biste konfigurirali isključenja za  **Windows server 2016 i 2019**, pročitajte članak [Konfiguriranje isključenja programa Microsoft Defender AntiVirus na servisu Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="bcd40-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="bcd40-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="bcd40-107">**Mac**</span></span>

<span data-ttu-id="bcd40-108">Pojedinosti o podržanim vrstama isključenosti i konfiguriranju popisa isključenja za Mac potražite u članku [podržane vrste isključenosti](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) te [kako konfigurirati popis isključenja](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="bcd40-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="bcd40-109">**Notes** Popise izuzeća možete provjeriti i pomoću datoteke za testiranje u programu EICAR.</span><span class="sxs-lookup"><span data-stu-id="bcd40-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="bcd40-110">Dodatne informacije potražite u članku [Provjera valjanosti popisa isključenja pomoću datoteke za testiranje u programu EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="bcd40-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="bcd40-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="bcd40-111">**Linux**</span></span>

<span data-ttu-id="bcd40-112">Pojedinosti o podržanim vrstama isključenosti i konfiguriranju popisa isključenja za Linuxom potražite u članku [podržane vrste isključenosti](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) i [Konfiguriranje i provjeru izuzetaka za Microsoft Defender ATP za Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="bcd40-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="bcd40-113">**Notes** Popise izuzeća možete provjeriti i pomoću datoteke za testiranje u programu EICAR.</span><span class="sxs-lookup"><span data-stu-id="bcd40-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="bcd40-114">Dodatne informacije potražite u članku [Provjera valjanosti popisa isključenja pomoću datoteke za testiranje u programu EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="bcd40-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 