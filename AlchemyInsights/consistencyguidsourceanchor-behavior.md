---
title: ConsistencyGuid / sourceAnchor ponašanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659583"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor ponašanja

Povezivanje Azure AD (verzija 1.1.524.0 i nakon) sada olakšava korištenje msDS ConsistencyGuid kao atribut sourceAnchor. Kada koristite tu značajku, Azure AD povezivanje automatski konfigurira pravila sinkronizacije:
  
- Koristite msDS ConsistencyGuid kao atribut sourceAnchor za objekte korisnika. ObjectGUID koristi se za druge vrste objekta.
    
- Za bilo koju dali lokalno AD korisnik objekt čije msDS ConsistencyGuid atribut nije popunjen, Azure zapisivanja AD povezivanje njegova vrijednost objectGUID natrag na msDS ConsistencyGuid atribut u Active Directory lokalno. Nakon popunjavaju msDS ConsistencyGuid atribut, Azure AD povezivanje Azure AD zatim izvozi objekt.
    
 **Napomena:** Jednom se lokalno AD objekt uvoze Azure AD povezivanje (koja je, uvezeni u AD poveznik prostora i predviđena u u Metaverse), više ne možete promijeniti njegova vrijednost sourceAnchor. Za određivanje vrijednosti sourceAnchor za u dao lokalno AD objekt, konfigurirajte njegov msDS ConsistencyGuid atribut prije je uvesti u Azure AD povezivanje. 
  
Dodatne informacije o SourceAnchor i ConsistencyGuid, pogledajte sljedeće: [Azure AD povezivanje: dizajniranje koncepti](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

