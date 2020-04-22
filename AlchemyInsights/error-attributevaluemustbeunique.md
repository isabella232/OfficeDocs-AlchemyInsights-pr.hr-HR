---
title: Pogreška AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703166"
---
# <a name="error-attributevaluemustbeunique"></a>Pogreška: AttributeValueMustBeUnique

Najčešći razlog za pogrešku AttributeValueMustBeUnique su dva objekta s različitim SourceAnchor (immutableId) imaju istu vrijednost za proxyaddresses i/ili UserPrincipalName atribute. Da biste riješili pogrešku AttributeValueMustBeUnique:
  
1. Identificirajte duplicirane proxyAddresses, userPrincipalName ili drugu vrijednost atributa koja uzrokuje pogrešku. Također odredite koja su dva (ili više) objekata uključena u sukob. Izvješće koje generira Azure AD Connect Health za sinkronizaciju može vam pomoći identificirati dva objekta.
    
2. Odredite koji bi objekt trebao i dalje imati dupliciranu vrijednost, a koji objekt ne bi trebao.
    
3. Uklonite dupliciranu vrijednost iz objekta koji NE bi trebao imati tu vrijednost. Imajte na umu da biste trebali napraviti promjenu u direktoriju iz kojeg je objekt izvor. U nekim ćete slučajevima možda morati izbrisati jedan od objekata u sukobu.
    
4. Ako ste napravili promjenu u lokalnom AD-u, neka Azure AD Connect sinkronizira promjenu za pogrešku da biste se popravili.
    

