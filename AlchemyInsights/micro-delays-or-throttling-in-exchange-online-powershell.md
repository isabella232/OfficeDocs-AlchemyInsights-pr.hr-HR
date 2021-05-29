---
title: Mikrokašnjenja ili ograničenja u komponenti Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702118"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrokašnjenja ili ograničenja u komponenti Exchange Online PowerShell

Prilikom izvođenja skripti i cmdleta u sustavu Exchange Online možda primijetite upozorenje o primjeni mikrokašnjenja ili kašnjenje. Evo nekoliko prijedloga kako to riješiti:

- Pokrenite našu dijagnostiku da biste opuštati pravilnike o ograničavanju ljuske PowerShell klijenta. Rješenje će za većinu riješiti problem.
- Ako problem i dalje nije riješen, [koristite modul komponente Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), koji obuhvaća CMDlete koji se temelje na REST API-ju i znatno su performantniji. To može biti odlično rješenje za brojne često korištene Get- cmdlete.
- Ako morate koristiti CMDlete koji nisu obuhvaćeni modulom v2, pročitajte running [PowerShell cmdlets](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)for large numbers of users in Office 365 , koji govori o tome kako se zaobilaže ograničenja ograničavanja komponente PowerShell u Exchange Online.
