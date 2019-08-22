---
title: Pogreška AttributeValueMustBeUnique
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526968"
---
# <a name="error-attributevaluemustbeunique"></a>Pogreška: AttributeValueMustBeUnique

Većinu uobičajenih razloga za AttributeValueMustBeUnique pogreške je dva objekte s različitim SourceAnchor (immutableId) imaju istu vrijednost atributa ProxyAddresses i/ili UserPrincipalName. Da biste ispravili pogrešku AttributeValueMustBeUnique:
  
1. Identificirati dupliciranu proxyAddresses, userPrincipalName ili druge vrijednosti atributa uzrokuje pogrešku. Također možete identificirati koji objekti dvije (ili više) uključen u sukobu. Izvješće generira Azure AD povezivanje stanja sustava za sinkronizaciju može vam pomoći prepoznati dvaju objekata.
    
2. Utvrdite koji objekt treba nastaviti s imaju dupliciranu vrijednost i ne bi trebala koji objekt.
    
3. Uklonite dupliciranu vrijednost iz objekt koji treba imati vrijednost. Imajte na umu treba napravite promjenu u imeniku gdje je izvorni objekt termini iz. U nekim slučajevima, morate izbrisati jedan od objekata u sukobu.
    
4. Izvršio promjenu u lokalno na AD omogućuju Azure povezivanje AD sinkronizacije promjena pogreška Dohvati nepromjenjive.
    

