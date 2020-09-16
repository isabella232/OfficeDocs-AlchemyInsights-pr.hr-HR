---
title: Potvrda domene
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734298"
---
# <a name="verify-your-domain"></a><span data-ttu-id="8f6d4-102">Potvrda domene</span><span class="sxs-lookup"><span data-stu-id="8f6d4-102">Verify your domain</span></span>

 <span data-ttu-id="8f6d4-103">**Zapis se vjerojatno nije ažurirao na internetu.**</span><span class="sxs-lookup"><span data-stu-id="8f6d4-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="8f6d4-104">Obično nam je potrebno samo nekoliko minuta da bismo mogli vidjeti novi zapis, no povremeno može potrajati i do nekoliko sati.</span><span class="sxs-lookup"><span data-stu-id="8f6d4-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="8f6d4-105">Ako ste već već dugo čekali, provjerite jeste li kopirali i zalijepili točnu vrijednost u zapis potvrde u programu TXT na hostiranju DNS-a.</span><span class="sxs-lookup"><span data-stu-id="8f6d4-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="8f6d4-106">Jedan od običnih problema nije uključujući dio zapisa "MS =".</span><span class="sxs-lookup"><span data-stu-id="8f6d4-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="8f6d4-107">I to nam je potrebno!</span><span class="sxs-lookup"><span data-stu-id="8f6d4-107">We need that too!</span></span>

- <span data-ttu-id="8f6d4-108">Na nekim hostima DNS-a morate poduzeti dodatni korak da biste spremili datoteku zone (gdje se pohranjuje DNS zapis) da bi se ažurirao na internetu.</span><span class="sxs-lookup"><span data-stu-id="8f6d4-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="8f6d4-109">Provjerite jeste li spremili promjene da bi Microsoft mogao vidjeti i potvrditi zapis.</span><span class="sxs-lookup"><span data-stu-id="8f6d4-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
