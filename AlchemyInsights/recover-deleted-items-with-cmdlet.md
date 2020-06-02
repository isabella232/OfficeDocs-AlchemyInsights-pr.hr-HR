---
title: Oporavak izbrisanih stavki s cmdletom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44492957"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="c5b96-102">Oporavak izbrisanih stavki s cmdletom</span><span class="sxs-lookup"><span data-stu-id="c5b96-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="c5b96-103">Koristite cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) za prikaz izbrisanih stavki u poštanskim sandučićima.</span><span class="sxs-lookup"><span data-stu-id="c5b96-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="c5b96-104">Nakon što pronađete izbrisane stavke, pomoću cmdleta [Restore-RecoverableItems vratite](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) ih.</span><span class="sxs-lookup"><span data-stu-id="c5b96-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="c5b96-105">Pogledajte sve pojedinosti u [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="c5b96-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="c5b96-106">Prije pokretanja ovog cmdleta morate biti dodijeljena uloga Izvoz uvoza poštanskog sandučića.</span><span class="sxs-lookup"><span data-stu-id="c5b96-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="c5b96-107">Dodatne informacije [potražite u odjeljku Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="c5b96-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
