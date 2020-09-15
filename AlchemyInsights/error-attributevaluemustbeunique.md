---
title: Pogreška prilikom Atributivaluelmustbeunique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709143"
---
# <a name="error-attributevaluemustbeunique"></a>Pogreška: Atributivaluelmustbeunique

Najčešći razlog pogreške atributa Attributevaluineunique jest dva objekta s drugačijim SourceAnchor (Imunotableid) imaju istu vrijednost za atribute Proxyadrese i/ili UserPrincipalName. Da biste riješili mogućnost dodijeljeno Atributevalubeunique:
  
1. Identificiraj duplicirane Proxyadrese, userPrincipalName ili neku drugu vrijednost atributa koja uzrokuje pogrešku. Odredite i koja su dva objekta (ili više) uključenih u sukob. Izvješće koje generira Azure AD Connect zdravlje za sinkronizaciju može vam pomoći identificirati dva objekta.
    
2. Odredite koji objekt mora nastaviti imati dupliciranu vrijednost, a koji objekt ne bi trebao.
    
3. Uklonite dupliciranu vrijednost iz objekta koji ne bi trebao imati tu vrijednost. Primjetite da biste trebali unijeti promjenu u direktorij iz kojeg je objekt izvor. U nekim slučajevima možda ćete morati izbrisati jedan od objekata u sukobu.
    
4. Ako ste unijeli promjenu u prostor za reklamu, neka Azure AD Connect sinkronizira promjenu pogreške radi ispravnosti.
    

