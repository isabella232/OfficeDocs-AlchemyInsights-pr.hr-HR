---
title: Snimanje poziva 1:1
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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314376"
---
# <a name="11-call-recording"></a>Snimanje poziva 1:1

Ako je **gumb Pokreni** snimanje zasivljen u pozivu u 1:1, morate promijeniti postavke pravilnika za utjecajnog korisnika. Da biste provjerili postavku pravilnika, pokrenite dijagnostiku za korisnika na koje se to utječe tako da **upišete Diag: Teams 1:1 Snimanje poziva.**     

Počevši od 31. svibnja 2021., započinjemo s novim pravilnikom Teams *pozivanja AllowCloudRecordingForCalls*. Prije te promjene snimanje poziva 1:1 kontrolira *AllowCloudRecording Teams* sastanaka. Ta je promjena dokumentirana u objavi Centra za poruke: [(Ažurirano) 1:1 Uvod u](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)pravilnik snimanja poziva .  

*AllowCloudRecordingForCalls*   Mogućnost pravilnika pozivanja po zadanom **je $False postavku.** Ako želite svim korisnicima blokirati snimanje poziva u 1:1, ne morate ništa poduzeti.  

Da biste svim korisnicima u 1:1 pozivima omogućili snimanje [poziva, Teams powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) za pokretanje sljedećeg cmdleta: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Možete i stvoriti novi pravilnik i postaviti **-AllowCloudRecordingForCalls** **da $true** i dodijeliti taj pravilnik korisnicima. 

Dodatne informacije potražite u članku Kontrole pravila snimanja poziva [1:1 Jesu (gotovo!) Ovdje .](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
