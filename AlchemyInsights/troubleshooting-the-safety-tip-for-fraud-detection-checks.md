---
title: Otklanjanje poteškoća sa sigurnosnim savjetom za provjere otkrivanja prijevara
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834723"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="40c02-102">Otklanjanje poteškoća sa sigurnosnim savjetom za provjere otkrivanja prijevara</span><span class="sxs-lookup"><span data-stu-id="40c02-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="40c02-103">Ako vam se prikaže savjet o sigurnosti na koji piše "Pošiljatelj nije uspio provjeriti naše provjere otkrivanja prijevare i možda nije onaj koji izgleda kao da je", pošiljatelj nije uspio proći provjere DKIM ili SPF provjere autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="40c02-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="40c02-104">Najbolji način rješavanja tog problema jest da pošiljatelj odobri sam sebe.</span><span class="sxs-lookup"><span data-stu-id="40c02-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="40c02-105">Ako pošiljatelj šalje u vaše ime, morate ih autorizirati dodavanjem IP adrese pošiljatelja u SPF zapis.</span><span class="sxs-lookup"><span data-stu-id="40c02-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="40c02-106">Dodatne [informacije potražite u članku Otklanjanje poteškoća s crvenim (sumnjivim) sigurnosnim savjetom](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) za provjeru otkrivanja prijevara.</span><span class="sxs-lookup"><span data-stu-id="40c02-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="40c02-107">Evo nekih drugih veza koje vam mogu pomoći:</span><span class="sxs-lookup"><span data-stu-id="40c02-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="40c02-108">Kako Microsoft koristi okvir pravilnika pošiljatelja (SPF) radi sprječavanja podvala</span><span class="sxs-lookup"><span data-stu-id="40c02-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="40c02-109">Postavljanje SPF-a radi sprječavanja podvala</span><span class="sxs-lookup"><span data-stu-id="40c02-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
