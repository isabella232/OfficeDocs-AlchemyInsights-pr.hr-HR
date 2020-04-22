---
title: Uvjetni pristup s intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706013"
---
# <a name="conditional-access-with-intune"></a>Uvjetni pristup s intune

Korištenje **uvjetnog pristupa** s intuneom zahtijeva 3 koraka: 
  
- Stvorite **pravila uvjetnog pristupa** koja definiraju koji su resursi zaštićeni i koji su uvjeti potrebni za pristup tim resursima. Na primjer, uređaj mora biti sukladan prije pristupanja korporativnoj e-pošti. 
    
- Stvorite **pravila usklađenosti** da biste definirali postavke koje se moraju ispuniti prije nego što se uređaj smatra sukladnim. Na primjer, uređaj mora imati pin od najmanje 6 znamenki prije nego što se smatra sukladnim. 
    
- Osiguravanje **pravila usklađenosti** i **pravila uvjetnog pristupa** usmjerene su na željene grupe korisnika. To može zahtijevati stvaranje određenih grupa korisnika u servisu Azure Active Directory. 
    
Opširnije::
  
- [Najbolji primjeri iz prakse za uvjetni pristup](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Prvi koraci s uvjetnim pristupom](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

