---
title: Provjerite vašu domenu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
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
ms.openlocfilehash: 3dd96a9731cfd75882dd3bb397005b19d471c882
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531351"
---
# <a name="verify-your-domain"></a><span data-ttu-id="9b7a0-102">Provjerite vašu domenu</span><span class="sxs-lookup"><span data-stu-id="9b7a0-102">Verify your domain</span></span>

 <span data-ttu-id="9b7a0-103">**Zapis vjerojatno prioritetna ažurira s Interneta.**</span><span class="sxs-lookup"><span data-stu-id="9b7a0-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="9b7a0-104">Obično potrebno je samo nekoliko minuta za nas moći vidjeti novi zapis, ali povremeno ga može potrajati nekoliko sati.</span><span class="sxs-lookup"><span data-stu-id="9b7a0-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="9b7a0-105">Ako ste koji već dugo waited, ponovno provjerite ste kopirati i zalijepiti točna vrijednost u TXT zapisu provjere na DNS domaćin.</span><span class="sxs-lookup"><span data-stu-id="9b7a0-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="9b7a0-106">Ne uključujući uobičajenih problema na "MS =" dio zapisa.</span><span class="sxs-lookup"><span data-stu-id="9b7a0-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="9b7a0-107">Moramo koji previše!</span><span class="sxs-lookup"><span data-stu-id="9b7a0-107">We need that too!</span></span>

- <span data-ttu-id="9b7a0-108">Na nekim hosts DNS morate poduzeti dodatni korak da biste spremili datoteku zone (DNS slog pohrane) tako da će se ažurirati s Interneta.</span><span class="sxs-lookup"><span data-stu-id="9b7a0-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="9b7a0-109">Uvjerite se da ste spremili promjene tako da Office 365 možete vidjeti i provjerite zapis.</span><span class="sxs-lookup"><span data-stu-id="9b7a0-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
