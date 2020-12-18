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
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Pogreške u sinkronizaciji Apple automatskog uključivanja uređaja

"Primijetili smo da imate jedan ili više tokena za ADE/DEP koji se nalaze u stanju pogreške. Dok ne riješite stanje pogreške za svaki pogođeni token, funkcija ADE neće funkcionirati za isto ".

Ta se pogreška može manifestirati na nekoliko načina, uključujući sljedeće:

1. Uređaji se ne mogu sinkronizirati sa servisa ABM/ASM do Intune
2. Zakazivanje zadataka profila za upis može neuspjeti
3. Uređaji možda neće uspješno dovršiti upis u ADU

Provjerite je li pogreška u sinkronizaciji prijavljena u konzoli za umetanje u odjeljku **uređaji > prijavite uređaje > unos Apple-a > tokeni programa za upis** i pregledajte sljedeću dokumentaciju da biste vidjeli bilo koje potencijalno zbrinjavanje:

[Pogreške u sinkronizaciji ABM/ASM za iOS/iPadOS i macOS automatizirani tokeni za upis uređaja](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
