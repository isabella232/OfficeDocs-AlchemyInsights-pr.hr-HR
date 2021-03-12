---
title: 1:1 poziva na snimanje
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733841"
---
# <a name="11-call-recording"></a>1:1 poziva na snimanje

Administratori sada moraju poduzeti akciju da bi korisnicima omogućili snimanje 1:1 poziva.
 
Počevši od travnja 12, 2021, počet ćemo provoditi nove grupe za pozivanje pravilnika *Allowclouderecordingforpoziv*. 

Trenutno 1:1 mogućnosti snimanja poziva kontroliraju se pomoću mogućnosti *Allowcloudesnimanje* u pravilima sastanka timova. Ako je korisnicima dopušteno snimati sastanke timova, možete snimati i 1:1 poziva.

Ako želite onemogućiti svim korisnicima snimanje 1:1 poziva, ne morate poduzeti nikakve akcije. Mogućnost *Allowclouderecordingforza* pozivanje pravilnika bit će $FALSE po zadanom.

Ta je promjena dokumentirana u sljedećoj pošti u centru za poruke: [(obnovljeno) 1:1 Pozivanje pravilnika za snimanje poziva](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) da biste postavili mogućnost pravilnika za timove koje morate koristiti u [timovima PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**Da biste omogućili snimanje poziva u programu 1:1 pozivi:** Set-CsTeamsCallingPolicy-Identity Global-Allowcloud Recordingforpoziv $True

**Da biste onemogućili snimanje poziva u programu 1:1 pozivi:** Set-CsTeamsCallingPolicy-Identity Global-Allowcloud Recordingforpoziv $FALSE

