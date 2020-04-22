---
title: Provjera domene
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710435"
---
# <a name="verify-your-domain"></a>Provjera domene

 **Zapis se vjerojatno nije ažurirao na internetu.**
  
Obično nam treba samo nekoliko minuta da vidimo novi zapis, ali povremeno to može potrajati i do nekoliko sati. 
  
- Ako ste već toliko dugo čekali, provjerite jeste li kopirali i zalijepili točnu vrijednost u TXT zapis potvrde na servisu DNS host. Jedan od uobičajenih problema nije uključujući dio zapisa "MS=". I to nam treba!

- Na nekim hostovima DNS-a morate poduzeti dodatni korak da biste spremili datoteku zone (gdje je pohranjen DNS zapis) da bi se ažurirao na cijelom internetu. Provjerite jeste li spremili promjene da bi Microsoft mogao vidjeti i potvrditi zapis.
