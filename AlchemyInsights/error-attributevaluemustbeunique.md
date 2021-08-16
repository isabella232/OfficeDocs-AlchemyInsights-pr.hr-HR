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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002112"
---
# <a name="error-attributevaluemustbeunique"></a>Pogreška: AttributeValueMustBeUnique

Najčešći razlog pogreške AttributeValueMustBeUnique dva su objekta s različitim atributima SourceAnchor (immutableId) koji imaju istu vrijednost za atribute ProxyAddresses i/ili UserPrincipalName. Da biste ispravili pogrešku AttributeValueMustBeUnique:
  
1. Odredite duplicirane proxyAddresses, userPrincipalName ili neku drugu vrijednost atributa koja uzrokuje pogrešku. Također odredite koja su dva (ili više) objekta uključena u sukob. Izvješće koje generira Azure AD Povezivanje Stanje za sinkronizaciju može vam pomoći u prepoznavanju dvaju objekata.
    
2. Odredite koji objekt i dalje mora imati dupliciranu vrijednost, a koji objekt ne bi trebao.
    
3. Uklonite dupliciranu vrijednost iz objekta koji ne bi trebao imati tu vrijednost. Imajte na umu da biste trebali promijeniti direktorij iz kojeg je objekt izvor. U nekim ćete slučajevima možda morati izbrisati jedan od objekata u sukobu.
    
4. Ako ste promijenili u lokalnom AD-u, dopustite servisu Azure AD Povezivanje sinkronizaciju promjene da bi se pogreška popravila.
    

