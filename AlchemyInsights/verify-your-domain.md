---
title: Provjerite vašu domenu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d37cdae616fabd2813dc7c8074e94b05f0391d20
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279529"
---
# <a name="verify-your-domain"></a><span data-ttu-id="237a2-102">Provjerite vašu domenu</span><span class="sxs-lookup"><span data-stu-id="237a2-102">Verify your domain</span></span>

 <span data-ttu-id="237a2-103">**Zapis vjerojatno prioritetna ažurira s Interneta.**</span><span class="sxs-lookup"><span data-stu-id="237a2-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="237a2-104">Obično potrebno je samo nekoliko minuta za nas moći vidjeti novi zapis, ali povremeno ga može potrajati nekoliko sati.</span><span class="sxs-lookup"><span data-stu-id="237a2-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="237a2-p101">Ako ste koji već dugo waited, ponovno provjerite ste kopirati i zalijepiti točna vrijednost u TXT zapisu provjere na DNS domaćin. Ne uključujući uobičajenih problema na "MS =" dio zapisa. Moramo koji previše!</span><span class="sxs-lookup"><span data-stu-id="237a2-p101">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. One common issue is not including the "MS=" part of the record. We need that too!</span></span>
    
- <span data-ttu-id="237a2-p102">Na nekim hosts DNS morate poduzeti dodatni korak da biste spremili datoteku zone (DNS slog pohrane) tako da će se ažurirati s Interneta. Uvjerite se da ste spremili promjene tako da Office 365 možete vidjeti i provjerite zapis.</span><span class="sxs-lookup"><span data-stu-id="237a2-p102">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet. Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

