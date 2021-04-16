---
title: Za javna grupa za migraciju mapa sa statusom CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812456"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Za javna grupa za migraciju mapa sa statusom CompletedWithErrors

Da biste dovršili skup, preskočite velike/loše stavke pomoću sljedećih koraka: 
1. Odobravanje preskočenih stavki u skupu za migraciju:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Pomoću sljedeće naredbe odobrite preskočene stavke na zahtjevima za migraciju koje su "Sinkronizirane", ali nisu dovršene:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Grupa za migraciju i zahtjevi trebali bi se nastaviti i dovršiti za nekoliko minuta.

