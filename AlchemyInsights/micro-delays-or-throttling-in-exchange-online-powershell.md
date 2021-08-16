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
ms.openlocfilehash: 6753dcb375ea5e19b01c4350b61aa8904aa102112df175a3f70281d18a634dbf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098558"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrokašnjenja ili ograničenja u komponenti Exchange Online PowerShell

Prilikom izvođenja skripti i cmdleta u sustavu Exchange Online možda primijetite upozorenje o primjeni mikrokašnjenja ili kašnjenje. Evo nekoliko prijedloga kako to riješiti:

- Pokrenite našu dijagnostiku da biste opuštati pravilnike o ograničavanju ljuske PowerShell klijenta. Rješenje će za većinu riješiti problem.
- Ako problem i dalje nije riješen, [koristite modul komponente Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), koji obuhvaća CMDlete koji se temelje na REST API-ju i znatno su performantniji. To može biti odlično rješenje za brojne često korištene Get- cmdlete.
- Ako morate koristiti CMDlete koji nisu obuhvaćeni modulom v2, pročitajte running [PowerShell cmdlets](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)for large numbers of users in Office 365 , koji govori o tome kako se zaobilaže ograničenja ograničavanja komponente PowerShell u Exchange Online.
