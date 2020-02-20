---
title: Vraćanje izbrisane javne mape
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
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158485"
---
# <a name="restore-a-deleted-public-folder"></a>Vraćanje izbrisane javne mape

**Da biste vratili izbrisane stavke iz javne mape:**

- Pogledajte [Ne možete oporaviti izbrisane stavke iz javne mape koja nije pošta u programu Outlook 2016](https://aka.ms/pfrec).
 
**Da biste vratili izbrisanu javnu mapu (bilo koje vrste)**: 

- Koristite sljedeću naredbu EXO PowerShell:

    Sintaksa:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Primjer: Sljedeća naredba vratit će podmapu1 i postaviti je pod \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Dodatne informacije [potražite u odjeljku Vraćanje izbrisane javne mape.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
