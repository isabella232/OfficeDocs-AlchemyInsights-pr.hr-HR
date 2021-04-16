---
title: Priprema za upotrebu protokola TLS 1.2 u okruženju Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085896"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="ba587-102">Priprema za upotrebu protokola TLS 1.2 u okruženju Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ba587-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="ba587-103">Od 31. listopada 2018. Microsoft 365 nastavit će s prijelazom na TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="ba587-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="ba587-104">Od 15. listopada 2020., O365 će početi ukidanje TLS 1.0 i 1.1 u cijelom servisu.</span><span class="sxs-lookup"><span data-stu-id="ba587-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="ba587-105">Uvođenje te promjene nastavit će se tijekom sljedećih nekoliko tjedana i mjeseci, no korisnici ne bi trebali preuzimati pozive TLS 1.0/1.1 kada se angažiraju s O365 počevši od 15. listopada 2020.</span><span class="sxs-lookup"><span data-stu-id="ba587-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="ba587-106">Kao što je prethodno priopćano (MC126199 u prosincu 2017., MC128929 u veljači 2018., MC186827 u srpnju 2019. i MC218794 u srpnju 2020.), sve naše internetske servise premještamo u sigurnost sloja transporta (TLS) 1,2+ da bismo pružili najbolje šifriranje u klasi te da bismo bili sigurniji.</span><span class="sxs-lookup"><span data-stu-id="ba587-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="ba587-107">Korisnici i dalje mogu odabrati da TLS 1.0/1.1 na svojim poslužiteljima i resursima, ali pretpostavljaju da će samo TLS 1.2 ili noviji funkcionirati prilikom interakcije s resursima sustava O365.</span><span class="sxs-lookup"><span data-stu-id="ba587-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="ba587-108">Dodatne informacije o tim promjenama potražite ovdje [i](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) [ovdje.](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="ba587-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  