---
title: Za javnu mapu migracije batch sa StatusOm CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043573"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Za javnu mapu migracije batch sa StatusOm CompletedWithErrors

Da biste dovršili seriju, preskočite velike/loše artikle, slijedite ove korake: 
1. Odobrite preskočene artikle na seriji migracije:

    Naziv serije \<Set-MigrationBatch> -ApprovePreskočene stavke 
2. Koristite sljedeću naredbu da biste odobrili preskočene stavke na zahtjevima za migraciju koji su "Sinkronizirani", ali nisu dovršeni:

    $pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i u $pf) {ako ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -PpedItemApprovalTime $([DateTime]::UtcNow)}}
3. Serija migracija i zahtjevi trebali bi se nastaviti i dovršiti za nekoliko minuta.

