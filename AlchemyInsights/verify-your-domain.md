---
title: Potvrda domene
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770983"
---
# <a name="verify-your-domain"></a><span data-ttu-id="05098-102">Potvrda domene</span><span class="sxs-lookup"><span data-stu-id="05098-102">Verify your domain</span></span>

 <span data-ttu-id="05098-103">**Zapis se vjerojatno nije ažurirao na internetu.**</span><span class="sxs-lookup"><span data-stu-id="05098-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="05098-104">Da bismo mogli vidjeti novi zapis, obično nam je potrebno samo nekoliko minuta, no katkad može potrajati i nekoliko sati.</span><span class="sxs-lookup"><span data-stu-id="05098-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="05098-105">Ako ste već dugo čekali, dvaput provjerite kopirate li i zalijepite točnu vrijednost u TXT zapis provjere valjanosti kod davatelja usluge hostiranja DNS-a.</span><span class="sxs-lookup"><span data-stu-id="05098-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="05098-106">Jedan od najčešćih problema nije uključivanje dijela zapisa "MS=".</span><span class="sxs-lookup"><span data-stu-id="05098-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="05098-107">I to nam je potrebno!</span><span class="sxs-lookup"><span data-stu-id="05098-107">We need that too!</span></span>

- <span data-ttu-id="05098-108">Kod nekih davatelja usluga hostiranja DNS-a morate poduzeti dodatni korak da biste spremili datoteku zone (gdje je pohranjen DNS zapis) da bi se ažurirao putem interneta.</span><span class="sxs-lookup"><span data-stu-id="05098-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="05098-109">Provjerite jeste li spremili promjene da bi Microsoft mogao vidjeti i potvrditi zapis.</span><span class="sxs-lookup"><span data-stu-id="05098-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
