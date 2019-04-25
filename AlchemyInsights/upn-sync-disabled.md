---
title: UPN sinkronizaciju onemogućen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423535"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="1b9ad-102">UPN sinkronizaciju onemogućen</span><span class="sxs-lookup"><span data-stu-id="1b9ad-102">UPN sync disabled</span></span>

<span data-ttu-id="1b9ad-103">Ako ste pokrenuli sinkroniziranje Azure AD prije 30 ožujak, 2016, pokrenite sljedeće Azure AD PowerShell cmdlet da biste omogućili UPN meki podudaranje za organizaciju samo:</span><span class="sxs-lookup"><span data-stu-id="1b9ad-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="1b9ad-104">**Skup MsolDirSyncFeature-značajka EnableSoftMatchOnUpn-omogućiti $True**</span><span class="sxs-lookup"><span data-stu-id="1b9ad-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="1b9ad-105">Podudaranje meki UPN automatski uključena za organizacije pokrenut sinkroniziranje Azure AD ili nakon ožujak 30, 2016.</span><span class="sxs-lookup"><span data-stu-id="1b9ad-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="1b9ad-106">Da biste saznali više o omogućavanju meki podudaranje na UPN i ostale značajke sinkronizacije, pogledajte [značajke povezivanje Azure AD sinkronizaciju usluge](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="1b9ad-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

