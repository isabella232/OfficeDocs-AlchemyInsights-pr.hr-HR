---
title: Pogreške u sinkronizaciji Apple automatskog uključivanja uređaja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714691"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="27be5-102">Pogreške u sinkronizaciji Apple automatskog uključivanja uređaja</span><span class="sxs-lookup"><span data-stu-id="27be5-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="27be5-103">"Primijetili smo da imate jedan ili više tokena za ADE/DEP koji se nalaze u stanju pogreške.</span><span class="sxs-lookup"><span data-stu-id="27be5-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="27be5-104">Dok ne riješite stanje pogreške za svaki pogođeni token, funkcija ADE neće funkcionirati za isto ".</span><span class="sxs-lookup"><span data-stu-id="27be5-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="27be5-105">Ta se pogreška može manifestirati na nekoliko načina, uključujući sljedeće:</span><span class="sxs-lookup"><span data-stu-id="27be5-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="27be5-106">Uređaji se ne mogu sinkronizirati sa servisa ABM/ASM do Intune</span><span class="sxs-lookup"><span data-stu-id="27be5-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="27be5-107">Zakazivanje zadataka profila za upis može neuspjeti</span><span class="sxs-lookup"><span data-stu-id="27be5-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="27be5-108">Uređaji možda neće uspješno dovršiti upis u ADU</span><span class="sxs-lookup"><span data-stu-id="27be5-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="27be5-109">Provjerite je li pogreška u sinkronizaciji prijavljena u konzoli za umetanje u odjeljku **uređaji > prijavite uređaje > unos Apple-a > tokeni programa za upis** i pregledajte sljedeću dokumentaciju da biste vidjeli bilo koje potencijalno zbrinjavanje:</span><span class="sxs-lookup"><span data-stu-id="27be5-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="27be5-110">Pogreške u sinkronizaciji ABM/ASM za iOS/iPadOS i macOS automatizirani tokeni za upis uređaja</span><span class="sxs-lookup"><span data-stu-id="27be5-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
