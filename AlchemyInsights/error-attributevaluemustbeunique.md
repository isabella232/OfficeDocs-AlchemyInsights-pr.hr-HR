---
title: Pogreška koja se Pripisavemustbeunique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36526968"
---
# <a name="error-attributevaluemustbeunique"></a>Pogreška: Atributocjenjemustbeunique

Najčešći razlog za Atributprocjenemustbeunique pogreška su dva objekta s različitim SourceAnchor (immutableId) imaju istu vrijednost za atribute proxy, i/ili UserPrincipalName. Da biste popravili Atributprocjenemustbeunique pogreška:
  
1. Identificirajte duplicirane Proxyadrese, userPrincipalName ili drugu vrijednost atributa koja uzrokuje pogrešku. Također identificirajte koja su dva (ili više) objekata uključena u sukob. Izvješće generirano pomoću servisa Azure AD Connect Health za sinkronizaciju može vam pomoći identificirati dva objekta.
    
2. Odredite koji bi objekt trebao i dalje imati duplicirane vrijednosti i koji objekt ne bi trebao.
    
3. Uklonite duplicirane vrijednosti iz objekta koji ne bi trebao imati tu vrijednost. Napominjemo da biste trebali napraviti promjenu u imeniku iz kojeg potječe objekt. U nekim ćete slučajevima možda morati izbrisati jedan od objekata u sukobu.
    
4. Ako ste napravili promjenu u prostorijama AD, neka Azure AD Connect sinkronizira promjenu da bi se pogreška popravila.
    

