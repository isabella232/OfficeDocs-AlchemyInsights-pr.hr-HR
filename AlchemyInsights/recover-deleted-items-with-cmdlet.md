---
title: Oporavak izbrisanih stavki pomoću cmdleta
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
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741295"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="db655-102">Oporavak izbrisanih stavki pomoću cmdleta</span><span class="sxs-lookup"><span data-stu-id="db655-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="db655-103">Pomoću cmdleta [Nabavite-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) Prikažite izbrisane stavke u poštanskim sandučićima.</span><span class="sxs-lookup"><span data-stu-id="db655-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="db655-104">Kada pronađete izbrisane stavke, upotrijebite cmdlet [Vraćanje-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) da biste ih vratili.</span><span class="sxs-lookup"><span data-stu-id="db655-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="db655-105">Pogledajte sve pojedinosti u odjeljku [dohvaćanje-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="db655-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="db655-106">Da biste mogli pokrenuti ovaj cmdlet, morate mu dodijeliti ulogu uvoza izvoza poštanskih sandučića.</span><span class="sxs-lookup"><span data-stu-id="db655-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="db655-107">Da biste saznali više, pročitajte članak [dohvaćanje-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) .</span><span class="sxs-lookup"><span data-stu-id="db655-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
