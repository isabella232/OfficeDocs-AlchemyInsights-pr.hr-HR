---
title: Pogreška AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28280252"
---
# <a name="error-attributevaluemustbeunique"></a>Pogreška: AttributeValueMustBeUnique

Većinu uobičajenih razloga za AttributeValueMustBeUnique pogreške je dva objekte s različitim SourceAnchor (immutableId) imaju istu vrijednost atributa ProxyAddresses i/ili UserPrincipalName. Da biste ispravili pogrešku AttributeValueMustBeUnique:
  
1. Identificirati dupliciranu proxyAddresses, userPrincipalName ili druge vrijednosti atributa uzrokuje pogrešku. Također možete identificirati koji objekti dvije (ili više) uključen u sukobu. Izvješće generira Azure AD povezivanje stanja sustava za sinkronizaciju može vam pomoći prepoznati dvaju objekata.
    
2. Utvrdite koji objekt treba nastaviti s imaju dupliciranu vrijednost i ne bi trebala koji objekt.
    
3. Uklonite dupliciranu vrijednost iz objekt koji treba imati vrijednost. Imajte na umu treba napravite promjenu u imeniku gdje je izvorni objekt termini iz. U nekim slučajevima, morate izbrisati jedan od objekata u sukobu.
    
4. Izvršio promjenu u lokalno na AD omogućuju Azure povezivanje AD sinkronizacije promjena pogreška Dohvati nepromjenjive.
    

