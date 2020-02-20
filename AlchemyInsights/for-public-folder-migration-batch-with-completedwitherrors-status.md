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
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158591"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Za javnu mapu migracije batch sa StatusOm CompletedWithErrors

Da biste dovršili seriju, preskočite velike/loše artikle, slijedite ove korake: 
1. Odobrite preskočene artikle na seriji migracije:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Koristite sljedeću naredbu da biste odobrili preskočene stavke na zahtjevima za migraciju koji su "Sinkronizirani", ali nisu dovršeni:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Serija migracija i zahtjevi trebali bi se nastaviti i dovršiti za nekoliko minuta.

