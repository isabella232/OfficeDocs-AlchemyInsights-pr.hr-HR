---
title: Otklanjanje poteškoća s sigurnosnim vrhom za provjeru otkrivanja prijevara
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658402"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="1d15f-102">Otklanjanje poteškoća s sigurnosnim vrhom za provjeru otkrivanja prijevara</span><span class="sxs-lookup"><span data-stu-id="1d15f-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="1d15f-103">Ako dobivate sigurnosnu dojavu na kojoj piše: "pošiljatelj nije uspeo da otkrije provjeru prijevara i možda neće biti ono što izgleda", onda Pošiljatelj nije prošao ni DKIM ni SPF provjere autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="1d15f-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="1d15f-104">Najbolji način za rješavanje toga jest da se pošiljatelj autorizira.</span><span class="sxs-lookup"><span data-stu-id="1d15f-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="1d15f-105">Ako pošiljatelj šalje u vaše ime, morate ih odobriti dodavanjem IP adrese pošiljatelja u SPF zapis.</span><span class="sxs-lookup"><span data-stu-id="1d15f-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="1d15f-106">Dodatne informacije potražite [u članku Otklanjanje poteškoća s crvenim (sumnjivim) sigurnosnim vrhom za otkrivanje prijevare](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="1d15f-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="1d15f-107">Evo još nekih veza koje mogu pomoći:</span><span class="sxs-lookup"><span data-stu-id="1d15f-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="1d15f-108">Kako Microsoft koristi okvir pravilnik o pošiljatelju (SPF) da bi spriječio zavaravanje</span><span class="sxs-lookup"><span data-stu-id="1d15f-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="1d15f-109">Postavljanje SPF-a radi sprječavanja zavaravanja</span><span class="sxs-lookup"><span data-stu-id="1d15f-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
