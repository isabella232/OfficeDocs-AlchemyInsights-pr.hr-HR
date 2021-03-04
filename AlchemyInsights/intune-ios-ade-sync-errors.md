---
title: Pogreške u sinkronizaciji Apple automatskog uključivanja uređaja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448914"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="15754-102">Pogreške u sinkronizaciji Apple automatskog uključivanja uređaja</span><span class="sxs-lookup"><span data-stu-id="15754-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="15754-103">"Primijetili smo da imate jedan ili više tokena za ADE/DEP koji se nalaze u stanju pogreške.</span><span class="sxs-lookup"><span data-stu-id="15754-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="15754-104">Dok ne riješite stanje pogreške za svaki pogođeni token, funkcija ADE neće funkcionirati kao što je očekivano. ".</span><span class="sxs-lookup"><span data-stu-id="15754-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="15754-105">Ta se pogreška može manifestirati na nekoliko načina, uključujući sljedeće:</span><span class="sxs-lookup"><span data-stu-id="15754-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="15754-106">Uređaji se ne mogu sinkronizirati sa servisa ABM/ASM do Intune</span><span class="sxs-lookup"><span data-stu-id="15754-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="15754-107">Zakazivanje zadataka profila za upis može neuspjeti</span><span class="sxs-lookup"><span data-stu-id="15754-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="15754-108">Uređaji možda neće uspješno dovršiti upis u ADU</span><span class="sxs-lookup"><span data-stu-id="15754-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="15754-109">Provjerite je li pogreška u sinkronizaciji prijavljena u konzoli za umetanje u odjeljku **uređaji > prijavite uređaje > uvrštavanje jabuka > tokeni programa za upis**.</span><span class="sxs-lookup"><span data-stu-id="15754-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="15754-110">Jedan od najčešćih uzroka pogreške pri sinkronizaciji jest istekom tekućeg tokena.</span><span class="sxs-lookup"><span data-stu-id="15754-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="15754-111">U mnogim će slučajevima obnova zahvaćenog tokena razriješiti problem.</span><span class="sxs-lookup"><span data-stu-id="15754-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="15754-112">Ako vam je istekao jedan ili više žetona, pogledajte sljedeću dokumentaciju koja će vam pomoći da ih obnovite po potrebi:</span><span class="sxs-lookup"><span data-stu-id="15754-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="15754-113">Obnovu tokena za automatsko upisivanje uređaja</span><span class="sxs-lookup"><span data-stu-id="15754-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="15754-114">Uz to, možete vidjeti i sljedeću dokumentaciju da biste vidjeli mogućnosti sanacije za druge pogreške koje uzrokuju pogreške u sinkronizaciji tokena:</span><span class="sxs-lookup"><span data-stu-id="15754-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="15754-115">Pogreške u sinkronizaciji ABM/ASM za iOS/iPadOS i macOS automatizirani tokeni za upis uređaja</span><span class="sxs-lookup"><span data-stu-id="15754-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="15754-116">Pogreške u sinkronizaciji ABM/ASM za iOS/iPadOS i macOS automatizirani tokeni za upis uređaja</span><span class="sxs-lookup"><span data-stu-id="15754-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
