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
# <a name="restore-a-deleted-public-folder"></a>Vraćanje izbrisane javne mape

**Da biste vratili izbrisane stavke iz javne mape**:

- [Izbrisane stavke ne možete oporaviti iz javne mape koja nije pošta u programu Outlook 2016](https://aka.ms/pfrec).
 
**Da biste vratili izbrisanu javnu mapu (bilo koje vrste)**, učinite sljedeće: 

- Upotrijebite sljedeću naredbu EXO PowerShell:

    Sintaksa

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Primjer: sljedeća naredba vraćat će Subfolder1 i postaviti je u odjeljku \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Dodatne pojedinosti potražite [u članku vraćanje izbrisane javne mape](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
