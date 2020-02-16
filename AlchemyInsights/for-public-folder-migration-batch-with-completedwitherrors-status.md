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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="c03cb-102">Za javnu mapu migracije batch sa StatusOm CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="c03cb-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="c03cb-103">Da biste dovršili seriju, preskočite velike/loše artikle, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="c03cb-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="c03cb-104">Odobrite preskočene artikle na seriji migracije:</span><span class="sxs-lookup"><span data-stu-id="c03cb-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="c03cb-105">Naziv serije \<Set-MigrationBatch> -ApprovePreskočene stavke</span><span class="sxs-lookup"><span data-stu-id="c03cb-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="c03cb-106">Koristite sljedeću naredbu da biste odobrili preskočene stavke na zahtjevima za migraciju koji su "Sinkronizirani", ali nisu dovršeni:</span><span class="sxs-lookup"><span data-stu-id="c03cb-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="c03cb-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i u $pf) {ako ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -PpedItemApprovalTime $([DateTime]::UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="c03cb-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="c03cb-108">Serija migracija i zahtjevi trebali bi se nastaviti i dovršiti za nekoliko minuta.</span><span class="sxs-lookup"><span data-stu-id="c03cb-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

