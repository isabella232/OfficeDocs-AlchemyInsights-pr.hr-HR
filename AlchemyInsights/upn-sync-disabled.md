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
# <a name="upn-sync-disabled"></a>UPN sinkronizaciju onemogućen

Ako ste pokrenuli sinkroniziranje Azure AD prije 30 ožujak, 2016, pokrenite sljedeće Azure AD PowerShell cmdlet da biste omogućili UPN meki podudaranje za organizaciju samo:
  
 **Skup MsolDirSyncFeature-značajka EnableSoftMatchOnUpn-omogućiti $True**
  
Podudaranje meki UPN automatski uključena za organizacije pokrenut sinkroniziranje Azure AD ili nakon ožujak 30, 2016.
  
Da biste saznali više o omogućavanju meki podudaranje na UPN i ostale značajke sinkronizacije, pogledajte [značajke povezivanje Azure AD sinkronizaciju usluge](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

