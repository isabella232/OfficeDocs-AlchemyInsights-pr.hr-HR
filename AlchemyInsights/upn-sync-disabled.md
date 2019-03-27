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
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767212"
---
# <a name="upn-sync-disabled"></a>UPN sinkronizaciju onemogućen

Ako ste pokrenuli sinkroniziranje Azure AD prije 30 ožujak, 2016, pokrenite sljedeće Azure AD PowerShell cmdlet da biste omogućili UPN meki podudaranje za organizaciju samo:
  
 **Skup MsolDirSyncFeature-značajka EnableSoftMatchOnUpn-omogućiti $True**
  
Podudaranje meki UPN automatski uključena za organizacije pokrenut sinkroniziranje Azure AD ili nakon ožujak 30, 2016.
  
Da biste saznali više o omogućavanju meki podudaranje na UPN i ostale značajke sinkronizacije, pogledajte [značajke povezivanje Azure AD sinkronizaciju usluge](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

