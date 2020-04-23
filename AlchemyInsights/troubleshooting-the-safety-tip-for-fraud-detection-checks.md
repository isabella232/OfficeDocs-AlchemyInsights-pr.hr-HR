---
title: Rješavanje problema sa sigurnosnim savjetom za provjere otkrivanja prijevara
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759504"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="dbfa6-102">Rješavanje problema sa sigurnosnim savjetom za provjere otkrivanja prijevara</span><span class="sxs-lookup"><span data-stu-id="dbfa6-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="dbfa6-103">Ako primate sigurnosnu savjet u kojoj piše "Pošiljatelj nije uspio provjeriti otkrivanje prijevara i možda nije ono što se čini da je", pošiljatelj nije uspio proći dkim ili SPF provjere autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="dbfa6-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="dbfa6-104">Najbolji način za rješavanje ovog je za pošiljatelja da se ovlastiti.</span><span class="sxs-lookup"><span data-stu-id="dbfa6-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="dbfa6-105">Ako pošiljatelj šalje u vaše ime, morate ih odobriti dodavanjem IP adrese pošiljatelja u SPF zapis.</span><span class="sxs-lookup"><span data-stu-id="dbfa6-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="dbfa6-106">Dodatne informacije [potražite u članku Otklanjanje poteškoća s crvenom (sumnjivom) sigurnosnom savjetu.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)</span><span class="sxs-lookup"><span data-stu-id="dbfa6-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="dbfa6-107">Evo još nekih veza koje mogu pomoći:</span><span class="sxs-lookup"><span data-stu-id="dbfa6-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="dbfa6-108">Kako Microsoft koristi okvir pravila pošiljatelja (SPF) kako bi spriječio zavaravanje</span><span class="sxs-lookup"><span data-stu-id="dbfa6-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="dbfa6-109">Postavite SPF kako biste spriječili zavaravanje</span><span class="sxs-lookup"><span data-stu-id="dbfa6-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
