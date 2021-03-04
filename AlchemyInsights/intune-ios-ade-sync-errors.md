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
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Pogreške u sinkronizaciji Apple automatskog uključivanja uređaja

"Primijetili smo da imate jedan ili više tokena za ADE/DEP koji se nalaze u stanju pogreške. Dok ne riješite stanje pogreške za svaki pogođeni token, funkcija ADE neće funkcionirati kao što je očekivano. ".

Ta se pogreška može manifestirati na nekoliko načina, uključujući sljedeće:

1. Uređaji se ne mogu sinkronizirati sa servisa ABM/ASM do Intune
2. Zakazivanje zadataka profila za upis može neuspjeti
3. Uređaji možda neće uspješno dovršiti upis u ADU

Provjerite je li pogreška u sinkronizaciji prijavljena u konzoli za umetanje u odjeljku **uređaji > prijavite uređaje > uvrštavanje jabuka > tokeni programa za upis**.

Jedan od najčešćih uzroka pogreške pri sinkronizaciji jest istekom tekućeg tokena. U mnogim će slučajevima obnova zahvaćenog tokena razriješiti problem.

Ako vam je istekao jedan ili više žetona, pogledajte sljedeću dokumentaciju koja će vam pomoći da ih obnovite po potrebi:

[Obnovu tokena za automatsko upisivanje uređaja](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Uz to, možete vidjeti i sljedeću dokumentaciju da biste vidjeli mogućnosti sanacije za druge pogreške koje uzrokuju pogreške u sinkronizaciji tokena:

[Pogreške u sinkronizaciji ABM/ASM za iOS/iPadOS i macOS automatizirani tokeni za upis uređaja](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Pogreške u sinkronizaciji ABM/ASM za iOS/iPadOS i macOS automatizirani tokeni za upis uređaja](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
