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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044332"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behavior

Azure AD Povezivanje (verzija 1.1.524.0 i nakon toga) sada olakšava korištenje atributa msDS-ConsistencyGuid kao sourceAnchor. Kada koristite tu značajku, Azure AD Povezivanje automatski konfigurira pravila sinkronizacije na sljedeće:
  
- Koristite msDS-ConsistencyGuid kao atribut sourceAnchor za korisničke objekte. ObjectGUID se koristi za druge vrste objekata.
    
- Za bilo koji lokalni ad korisnički objekt čiji atribut msDS-ConsistencyGuid nije popunjen, Azure AD Povezivanje vraća vrijednost objectGUID na atribut msDS-ConsistencyGuid u lokalnom servisu Active Directory. Kada se popunjava atribut msDS-ConsistencyGuid, Azure AD Povezivanje zatim izvozi objekt u Azure AD.
    
 **Napomena:** Kada se lokalni AD objekt uvozi u Azure AD Povezivanje (to jest, uvozi se u prostor AD Connector i projiciran u Metaverse), više ne možete mijenjati njegovu izvornu vrijednostAnchor. Da biste odredili vrijednost sourceAnchor za određeni lokalni AD objekt, prije uvoza u Azure AD Povezivanje konfigurirajte atribut msDS-ConsistencyGuid. 
  
Dodatne informacije o sourceAnchoru i dosljednostiGuid potražite u sljedećem: [Azure AD Povezivanje: Koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

