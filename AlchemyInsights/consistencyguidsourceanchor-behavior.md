---
title: Ponašanje DosljednostGuid / sourceAnchor
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705725"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Ponašanje DosljednostGuid / sourceAnchor

Azure AD Connect (verzija 1.1.524.0 i nakon) sada olakšava korištenje msDS-DosljednostGuid kao atribut sourceAnchor. Kada koristite ovu značajku, Azure AD Connect automatski konfigurira pravila sinkronizacije na:
  
- Koristite msDS-DosljednostGuid kao atribut sourceAnchor za korisničke objekte. ObjectGUID se koristi za druge vrste objekata.
    
- Za sve dane lokalni objekt AD Korisnik čiji atribut msDS-DosljednostGuid nije popunjen, Azure AD Connect vraća svoju vrijednost objectGUID natrag na atribut msDS-DosljednostGuid u lokalnom servisu Active Directory. Nakon popunjavanja atributa msDS-DosljednostGuid, Azure AD Connect zatim izvozi objekt u Azure AD.
    
 **Napomena:** Nakon što se lokalni AD objekt uveze u Azure AD Connect (tj. uvozi u prostor AD poveznika i projicira u Metaverse), više ne možete promijeniti njegovu vrijednost sourceAnchor. Da biste odredili vrijednost sourceAnchor za određeni lokalni AD objekt, konfigurirajte njegov atribut msDS-DosljednostGuid prije uvoza u Azure AD Connect. 
  
Dodatne informacije o SourceAnchor i DosljednostGuid potražite u sljedećim [člancima Azure AD Connect: Koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

