---
title: Vraćanje izbrisane javne mape
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809431"
---
# <a name="restore-a-deleted-public-folder"></a>Vraćanje izbrisane javne mape

**Vraćanje izbrisanih stavki iz javne mape:**

- Pogledajte Ne možete oporaviti izbrisane stavke iz javne mape koja [nije e-pošta u programu Outlook 2016](https://aka.ms/pfrec).
 
**Da biste vratili izbrisanu javnu mapu (bilo koje vrste)**: 

- Upotrijebite sljedeću naredbu EXO PowerShell:

    Sintaksa:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Primjer: Sljedeća naredba vraća podmapu1 i smjestit će je u \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Dodatne [informacije potražite u članku Vraćanje izbrisane](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) javne mape.
