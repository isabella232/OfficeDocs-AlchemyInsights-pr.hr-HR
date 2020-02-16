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
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063610"
---
# <a name="restore-a-deleted-public-folder"></a>Vraćanje izbrisane javne mape

**Da biste vratili izbrisane stavke iz javne mape:**

- Pogledajte [Ne možete oporaviti izbrisane stavke iz javne mape koja nije pošta u programu Outlook 2016](https://aka.ms/pfrec).
 
**Da biste vratili izbrisanu javnu mapu (bilo koje vrste)**: 

- Koristite sljedeću naredbu EXO PowerShell:

    Sintaksa:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | {$_. Ime -eq "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity-Put gdje \<će mapa biti vraćena>

    Primjer: Sljedeća naredba vratit će podmapu1 i postaviti je pod \Parent1:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | {$_. Naziv -eq "Podmapa1"}; Postavi-PublicFolder $pf.identity -Put \Parent1

Dodatne informacije [potražite u odjeljku Vraćanje izbrisane javne mape.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
