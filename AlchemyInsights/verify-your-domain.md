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
# <a name="verify-your-domain"></a><span data-ttu-id="46460-102">Provjera domene</span><span class="sxs-lookup"><span data-stu-id="46460-102">Verify your domain</span></span>

 <span data-ttu-id="46460-103">**Zapis se vjerojatno nije ažurirao na internetu.**</span><span class="sxs-lookup"><span data-stu-id="46460-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="46460-104">Obično nam treba samo nekoliko minuta da vidimo novi zapis, ali povremeno to može potrajati i do nekoliko sati.</span><span class="sxs-lookup"><span data-stu-id="46460-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="46460-105">Ako ste već toliko dugo čekali, provjerite jeste li kopirali i zalijepili točnu vrijednost u TXT zapis potvrde na servisu DNS host.</span><span class="sxs-lookup"><span data-stu-id="46460-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="46460-106">Jedan od uobičajenih problema nije uključujući dio zapisa "MS=".</span><span class="sxs-lookup"><span data-stu-id="46460-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="46460-107">I to nam treba!</span><span class="sxs-lookup"><span data-stu-id="46460-107">We need that too!</span></span>

- <span data-ttu-id="46460-108">Na nekim hostovima DNS-a morate poduzeti dodatni korak da biste spremili datoteku zone (gdje je pohranjen DNS zapis) da bi se ažurirao na cijelom internetu.</span><span class="sxs-lookup"><span data-stu-id="46460-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="46460-109">Provjerite jeste li spremili promjene da bi Microsoft mogao vidjeti i potvrditi zapis.</span><span class="sxs-lookup"><span data-stu-id="46460-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
