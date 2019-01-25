---
title: Savjet sigurnost za otkrivanje prijevara za otklanjanje poteškoća provjerava
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29461751"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="23a7b-102">Savjet sigurnost za otkrivanje prijevara za otklanjanje poteškoća provjerava</span><span class="sxs-lookup"><span data-stu-id="23a7b-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="23a7b-p101">Ako ste prvi savjet sigurnost koji kaže "pošiljatelj nije uspjelo naše prijevara otkrivanje provjerava i možda nije tko pojavljuju se", a zatim pošiljatelj nije uspjelo proći provjere autentičnosti DKIM ili SPF. Za pošiljatelja da bi ovlastili same je najbolji način da biste riješili problem. Ako pošiljatelj slanja u vaše ime, morate Autorizirajte dodavanjem IP adresu pošiljatelja SPF zapisa.</span><span class="sxs-lookup"><span data-stu-id="23a7b-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="23a7b-106">Dodatne informacije potražite [Savjet crveni sigurnost (sumnjivih) za otkrivanje prijevara za otklanjanje poteškoća provjerava](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="23a7b-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="23a7b-107">Ovdje su neke veze koje mogu pomoći:</span><span class="sxs-lookup"><span data-stu-id="23a7b-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="23a7b-108">Kako Office 365 koristi pošiljatelja framework pravila (SPF) za onemogućavanje prikrivanja</span><span class="sxs-lookup"><span data-stu-id="23a7b-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="23a7b-109">Postavljanje SPF u Office 365 pomoći prikrivanja</span><span class="sxs-lookup"><span data-stu-id="23a7b-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

