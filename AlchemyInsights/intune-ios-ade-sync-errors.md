---
title: Pogreške prilikom sinkronizacije automatske prijave na Appleov uređaj
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013740"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Pogreške prilikom sinkronizacije automatske prijave na Appleov uređaj

"Otkrili smo da imate jedan ili više ADE/DEP tokena koji se nalaze u stanju pogreške. Dok se stanje pogreške ne riješi za svaki zahvaćeni token, funkcija ADE neće funkcionirati na očekivani način.".

Ta se pogreška može manifestirati na nekoliko načina, uključujući sljedeće:

1. Uređaji se možda neće sinkronizirati s uređaja ABM/ASM sa servisom Intune
2. Dodjele profila za prijavu možda ne uspijevaju
3. Uređaji možda neće uspješno dovršiti registraciju za ADE

Provjerite je li pogreška sinkronizacije prijavljena na konzoli Intune **u odjeljku Uređaji > Za prijavu uređaja > appleova > programskih tokena**.

Jedan od najčešćih uzroka pogreške prilikom sinkronizacije jest istek trenutnog tokena. U mnogim će slučajevima obnova zahvaćenog tokena riješiti problem.

Ako je jedan ili više tokena isteklo, pogledajte sljedeću dokumentaciju da biste ih po potrebi obnovili:

[Obnavljanje tokena za automatsku prijavu na uređaj](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Osim toga, možete vidjeti sljedeću dokumentaciju da biste vidjeli potencijalne otklanjanja drugih pogrešaka koje uzrokuju pogreške sinkronizacije tokena:

[Pogreške sinkronizacije sustava ABM/ASM za tokene za automatsku prijavu na iOS/iPadOS i macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Pogreške sinkronizacije sustava ABM/ASM za tokene za automatsku prijavu na iOS/iPadOS i macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
