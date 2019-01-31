---
title: UPN sinkronizaciju onemogućen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657963"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="27713-102">UPN sinkronizaciju onemogućen</span><span class="sxs-lookup"><span data-stu-id="27713-102">UPN sync disabled</span></span>

<span data-ttu-id="27713-103">Ako ste pokrenuli sinkroniziranje Azure AD prije 30 ožujak, 2016, pokrenite sljedeće Azure AD PowerShell cmdlet da biste omogućili UPN meki podudaranje za organizaciju samo:</span><span class="sxs-lookup"><span data-stu-id="27713-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="27713-104">**Skup MsolDirSyncFeature-značajka EnableSoftMatchOnUpn-omogućiti $True**</span><span class="sxs-lookup"><span data-stu-id="27713-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="27713-105">Podudaranje meki UPN automatski uključena za organizacije pokrenut sinkroniziranje Azure AD ili nakon ožujak 30, 2016.</span><span class="sxs-lookup"><span data-stu-id="27713-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="27713-106">Da biste saznali više o omogućavanju meki podudaranje na UPN i ostale značajke sinkronizacije, pogledajte [značajke povezivanje Azure AD sinkronizaciju usluge](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="27713-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

