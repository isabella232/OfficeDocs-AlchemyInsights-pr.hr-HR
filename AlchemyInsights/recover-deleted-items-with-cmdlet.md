---
title: Oporavak izbrisanih stavki pomoću cmdleta
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835803"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="828f3-102">Oporavak izbrisanih stavki pomoću cmdleta</span><span class="sxs-lookup"><span data-stu-id="828f3-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="828f3-103">Pomoću [cmdleta Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) pregledavajte izbrisane stavke u poštanskim sandučićima.</span><span class="sxs-lookup"><span data-stu-id="828f3-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="828f3-104">Kada pronađete izbrisane stavke, pomoću cmdleta [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) možete ih vratiti.</span><span class="sxs-lookup"><span data-stu-id="828f3-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="828f3-105">Pogledajte sve detalje u [odjeljku Get-RecoverableItems (Get-RecoverableItems).](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="828f3-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="828f3-106">Da biste mogli pokrenuti ovaj cmdlet, morate imati ulogu Uvoz uvoza poštanskog sandučića.</span><span class="sxs-lookup"><span data-stu-id="828f3-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="828f3-107">Dodatne informacije [potražite u članku Get-RecoverableItems (Get-RecoverableItems).](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="828f3-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
