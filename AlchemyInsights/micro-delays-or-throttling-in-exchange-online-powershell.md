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
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314692"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrokašnjenja ili ograničenja u komponenti Exchange Online PowerShell

Prilikom izvođenja skripti i cmdleta u sustavu Exchange Online možda primijetite upozorenje o primjeni mikrokašnjenja ili kašnjenje. Evo nekoliko prijedloga kako to riješiti:

- Pokrenite našu dijagnostiku da biste opuštati pravilnike o ograničavanju ljuske PowerShell klijenta. Rješenje će za većinu riješiti problem.
- Ako problem i dalje nije riješen, [koristite modul komponente Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), koji obuhvaća CMDlete koji se temelje na REST API-ju i znatno su performantniji. To može biti odlično rješenje za brojne često korištene Get- cmdlete.
- Ako morate koristiti CMDlete koji nisu obuhvaćeni modulom v2, pročitajte running [PowerShell cmdlets](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)for large numbers of users in Office 365 , koji govori o tome kako se zaobilaže ograničenja ograničavanja komponente PowerShell u Exchange Online.
