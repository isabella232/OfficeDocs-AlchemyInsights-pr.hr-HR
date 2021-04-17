---
title: ConsistencyGuid / sourceAnchor behavior
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816984"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behavior

Azure AD Connect (verzija 1.1.524.0 i nakon toga) sada olakšava korištenje atributa msDS-ConsistencyGuid kao atribut sourceAnchor. Kada koristite tu značajku, Azure AD Connect automatski konfigurira pravila sinkronizacije na sljedeće:
  
- Koristite msDS-ConsistencyGuid kao atribut sourceAnchor za korisničke objekte. ObjectGUID se koristi za druge vrste objekata.
    
- Za bilo koji lokalni ad korisnički objekt čiji atribut msDS-ConsistencyGuid nije popunjen, Azure AD Connect vraća vrijednost objectGUID na atribut msDS-ConsistencyGuid u lokalnom servisu Active Directory. Kada se popunjava atribut msDS-ConsistencyGuid, Azure AD Connect zatim izvozi objekt u Azure AD.
    
 **Napomena:** Kada se lokalni AD objekt uvozi u Azure AD Connect (to jest, uvozi se u prostor ad connectora i projiciran u Metaverse), više ne možete mijenjati njegovu izvornu vrijednostAnchor. Da biste odredili vrijednost sourceAnchor za određeni lokalni AD objekt, prije uvoza u Azure AD Connect konfigurirajte atribut msDS-ConsistencyGuid. 
  
Dodatne informacije o sourceAnchoru i dosljednostiGuid potražite u sljedećem: [Azure AD Connect: koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

