---
title: Error AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813752"
---
# <a name="error-attributevaluemustbeunique"></a>Pogreška: AttributeValueMustBeUnique

Najčešći razlog pogreške AttributeValueMustBeUnique dva su objekta s različitim atributima SourceAnchor (immutableId) koji imaju istu vrijednost za atribute ProxyAddresses i/ili UserPrincipalName. Da biste ispravili pogrešku AttributeValueMustBeUnique:
  
1. Odredite duplicirane proxyAddresses, userPrincipalName ili neku drugu vrijednost atributa koja uzrokuje pogrešku. Također odredite koja su dva (ili više) objekta uključena u sukob. Izvješće koje generira Azure AD Connect Health za sinkronizaciju može vam pomoći da identificirate ta dva objekta.
    
2. Odredite koji objekt i dalje mora imati dupliciranu vrijednost, a koji objekt ne bi trebao.
    
3. Uklonite dupliciranu vrijednost iz objekta koji ne bi trebao imati tu vrijednost. Imajte na umu da biste trebali promijeniti direktorij iz kojeg je objekt izvor. U nekim ćete slučajevima možda morati izbrisati jedan od objekata u sukobu.
    
4. Ako ste promijenili u lokalnom AD-u, dopustite servisu Azure AD Connect sinkronizaciju promjene da bi se pogreška popravila.
    

