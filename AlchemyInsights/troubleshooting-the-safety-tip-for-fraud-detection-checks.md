---
title: Otklanjanje poteškoća sa sigurnosnim savjetom za provjere otkrivanja prijevara
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
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504975"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="f23bd-102">Otklanjanje poteškoća sa sigurnosnim savjetom za provjere otkrivanja prijevara</span><span class="sxs-lookup"><span data-stu-id="f23bd-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="f23bd-103">Ako ste uzimajući sigurnost savjet taj kaže " pošiljatelj nije ispunilo proročanstvo naš prijevara otkrivanje ček i možda ne biti tko oni pojaviti se biti", onda pošiljatelj nije ispunilo proročanstvo to dobar uspijeh oba DKIM ili SPF sigurnost ček.</span><span class="sxs-lookup"><span data-stu-id="f23bd-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="f23bd-104">Najbolji način za rješavanje je za pošiljatelja da se ovlastiti.</span><span class="sxs-lookup"><span data-stu-id="f23bd-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="f23bd-105">Ako pošiljatelj šalje u vaše ime, morate ih ovlastiti dodavanjem IP adrese pošiljatelja u vaš SPF zapis.</span><span class="sxs-lookup"><span data-stu-id="f23bd-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="f23bd-106">Dodatne informacije [potražite u odjeljku Otklanjanje poteškoća s crvenom (sumnjivom) sigurnosnom šašamca.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)</span><span class="sxs-lookup"><span data-stu-id="f23bd-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="f23bd-107">Evo nekih drugih veza koje vam mogu pomoći:</span><span class="sxs-lookup"><span data-stu-id="f23bd-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="f23bd-108">Kako Microsoft koristi okvir pravila pošiljatelja (SPF) za sprječavanje zavaravanja</span><span class="sxs-lookup"><span data-stu-id="f23bd-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="f23bd-109">Postavljanje SPF-a radi sprječavanja zavaravanja</span><span class="sxs-lookup"><span data-stu-id="f23bd-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
