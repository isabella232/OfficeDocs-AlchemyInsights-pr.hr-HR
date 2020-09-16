---
title: Funkcija ConsistencyGuid/sourceanchor
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756275"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Funkcija ConsistencyGuid/sourceanchor

Azure AD Connect (verzija 1.1.524.0 i nakon) sada olakšava korištenje servisa msDS-ConsistencyGuid kao atributa sourceAnchor. Kada koristite ovu značajku, Azure AD Connect automatski konfigurira pravila sinkronizacije na sljedeće:
  
- Koristite msDS-ConsistencyGuid kao atribut sourceAnchor za korisničke objekte. ObjectGUID se koristi za druge vrste objekata.
    
- Za bilo koji lokalni objekt oglasa za korisnike čiji atribut msDS-ConsistencyGuid nije popunjen, Azure AD Connect zapisuje vrijednost objectGUID natrag u atribut msDS-ConsistencyGuid u lokalnom servisu Active Directory. Kada se atribut msDS-ConsistencyGuid popunjava, Azure AD Connect zatim izvozi objekt na Azure AD.
    
 **Upozorenje:** Kada se lokalni oglasni objekt uvozi u Azure AD Connect (to jest, uvezen u prostor OGLASNOG poveznika i projiciran na metaverse), više ne možete promijeniti vrijednost funkcije sourceAnchor. Da biste naveli vrijednost sourceAnchor za navedeni lokalni objekt oglasa, konfigurirajte atribut msDS-ConsistencyGuid prije uvoza u Azure AD Connect. 
  
Dodatne informacije o SourceAnchor i ConsistencyGuid-u potražite u sljedećim člancima: [Azure ad Connect: koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

