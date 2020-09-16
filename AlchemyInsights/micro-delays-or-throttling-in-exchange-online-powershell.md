---
title: Mikrokašnjenja ili ograničenja u komponenti Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 55844747be27ea4ff8f538492e576195b3a5f0bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743906"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrokašnjenja ili ograničenja u komponenti Exchange Online PowerShell

Prilikom izvođenja skripti i cmdleta u sustavu Exchange Online možda primijetite upozorenje o primjeni mikrokašnjenja ili kašnjenje. U nastavku su navedena dva s tim povezana prijedloga:

- Možete pokušati koristiti [modul Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), koji obuhvaća cmdlete koji se temelje na REST API-ju i imaju znatno bolje performanse. To može biti odlično rješenje za brojne često korištene Get- cmdlete.
- Ako morate koristiti cmdlete koji još nisu obuhvaćeni modulom v2, pročitajte članak [Pokretanje cmdleta za PowerShell za velik broj korisnika u sustavu Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), koji govori o zaobilaženju očekivanih ograničenja propusnosti u komponenti PowerShell u sustavu Exchange Online.
