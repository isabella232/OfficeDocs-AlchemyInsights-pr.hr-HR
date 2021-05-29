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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="4d896-102">Mikrokašnjenja ili ograničenja u komponenti Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="4d896-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="4d896-103">Prilikom izvođenja skripti i cmdleta u sustavu Exchange Online možda primijetite upozorenje o primjeni mikrokašnjenja ili kašnjenje.</span><span class="sxs-lookup"><span data-stu-id="4d896-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="4d896-104">Evo nekoliko prijedloga kako to riješiti:</span><span class="sxs-lookup"><span data-stu-id="4d896-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="4d896-105">Pokrenite našu dijagnostiku da biste opuštati pravilnike o ograničavanju ljuske PowerShell klijenta.</span><span class="sxs-lookup"><span data-stu-id="4d896-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="4d896-106">Rješenje će za većinu riješiti problem.</span><span class="sxs-lookup"><span data-stu-id="4d896-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="4d896-107">Ako problem i dalje nije riješen, [koristite modul komponente Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), koji obuhvaća CMDlete koji se temelje na REST API-ju i znatno su performantniji.</span><span class="sxs-lookup"><span data-stu-id="4d896-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="4d896-108">To može biti odlično rješenje za brojne često korištene Get- cmdlete.</span><span class="sxs-lookup"><span data-stu-id="4d896-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="4d896-109">Ako morate koristiti CMDlete koji nisu obuhvaćeni modulom v2, pročitajte running [PowerShell cmdlets](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)for large numbers of users in Office 365 , koji govori o tome kako se zaobilaže ograničenja ograničavanja komponente PowerShell u Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="4d896-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
