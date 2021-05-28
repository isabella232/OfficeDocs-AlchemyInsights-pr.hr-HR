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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696914"
---
# <a name="11-call-recording"></a>Snimanje poziva 1:1

Ako je **gumb Pokreni** snimanje zasivljen u pozivu u 1:1, morate promijeniti postavke pravilnika za utjecajnog korisnika.   

Počevši od 31. svibnja 2021., započinjemo s novim pravilnikom Teams *pozivanja AllowCloudRecordingForCalls*. Prije te promjene snimanje poziva 1:1 kontrolira *AllowCloudRecording Teams* sastanaka. Ta je promjena dokumentirana u objavi Centra za poruke: [(Ažurirano) 1:1 Uvod pravilnika za snimanje poziva](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   Mogućnost pravilnika pozivanja postavljena **je na $False po** zadanom. Ako želite svim korisnicima blokirati snimanje poziva u 1:1, ne morate ništa poduzeti.  

Da biste omogućili snimanje poziva za sve korisnike u 1:1 pozivima, Teams PowerShell za pokretanje sljedećeg cmdleta: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Možete i stvoriti novi pravilnik i postaviti **-AllowCloudRecordingForCalls** **tako da $true** i dodijeliti taj pravilnik korisnicima. 

Dodatne informacije potražite u članku Kontrole pravila snimanja poziva [1:1 Jesu (gotovo!) Ovdje .](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
