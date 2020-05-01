---
title: Mikrokašnjenja ili ograničenja u komponenti Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947797"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="95408-102">Mikrokašnjenja ili ograničenja u komponenti Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="95408-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="95408-103">Prilikom izvođenja skripti i cmdleta u sustavu Exchange Online možda primijetite upozorenje o primjeni mikrokašnjenja ili kašnjenje.</span><span class="sxs-lookup"><span data-stu-id="95408-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="95408-104">U nastavku su navedena dva s tim povezana prijedloga:</span><span class="sxs-lookup"><span data-stu-id="95408-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="95408-105">Možete pokušati koristiti [modul Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), koji obuhvaća cmdlete koji se temelje na REST API-ju i imaju znatno bolje performanse.</span><span class="sxs-lookup"><span data-stu-id="95408-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="95408-106">To može biti odlično rješenje za brojne često korištene Get- cmdlete.</span><span class="sxs-lookup"><span data-stu-id="95408-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="95408-107">Ako morate koristiti cmdlete koji još nisu obuhvaćeni modulom v2, pročitajte članak [Pokretanje cmdleta za PowerShell za velik broj korisnika u sustavu Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), koji govori o zaobilaženju očekivanih ograničenja propusnosti u komponenti PowerShell u sustavu Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="95408-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
