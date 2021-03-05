---
title: Onemogućivanje mrežnog skeniranja
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481125"
---
# <a name="disable-network-scan"></a><span data-ttu-id="6fc0e-102">Onemogućivanje mrežnog skeniranja</span><span class="sxs-lookup"><span data-stu-id="6fc0e-102">Disable network scan</span></span>

<span data-ttu-id="6fc0e-103">Skeniranje mrežnih dionica može utjecati na performanse.</span><span class="sxs-lookup"><span data-stu-id="6fc0e-103">Network share scans may impact performance.</span></span>  <span data-ttu-id="6fc0e-104">Da biste osigurali da klijent ne skenira mrežne dionice/datoteke po zadanom, konfigurirajte sljedeće postavke u aplikaciji programa Windows Defender da biste učinili **istinu**:</span><span class="sxs-lookup"><span data-stu-id="6fc0e-104">To ensure the client does not scan network shares/files by default, configure the following settings in the Windows Defender application to **True**:</span></span>

- <span data-ttu-id="6fc0e-105">Otklanjanje poteškoća s računalima</span><span class="sxs-lookup"><span data-stu-id="6fc0e-105">DisableScanningMappedNetworkDrivesForFullScan</span></span>
- <span data-ttu-id="6fc0e-106">DisableScanningNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="6fc0e-106">DisableScanningNetworkFiles</span></span>