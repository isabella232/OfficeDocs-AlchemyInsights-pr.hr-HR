---
title: Vraćanje izbrisane javne mape
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774523"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="50041-102">Vraćanje izbrisane javne mape</span><span class="sxs-lookup"><span data-stu-id="50041-102">Restore a deleted public folder</span></span>

<span data-ttu-id="50041-103">**Da biste vratili izbrisane stavke iz javne mape**:</span><span class="sxs-lookup"><span data-stu-id="50041-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="50041-104">[Izbrisane stavke ne možete oporaviti iz javne mape koja nije pošta u programu Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="50041-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="50041-105">**Da biste vratili izbrisanu javnu mapu (bilo koje vrste)**, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="50041-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="50041-106">Upotrijebite sljedeću naredbu EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="50041-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="50041-107">Sintaksa</span><span class="sxs-lookup"><span data-stu-id="50041-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="50041-108">Primjer: sljedeća naredba vraćat će Subfolder1 i postaviti je u odjeljku \Parent1:</span><span class="sxs-lookup"><span data-stu-id="50041-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="50041-109">Dodatne pojedinosti potražite [u članku vraćanje izbrisane javne mape](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="50041-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
