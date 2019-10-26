---
title: Ponašanje za Konzistenceguid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36516965"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Ponašanje za Konzistenceguid/sourceAnchor

Azure AD Connect (verzija 1.1.524.0 i after) sada olakšava korištenje atributa msDS- Kada koristite ovu značajku, Azure AD Connect automatski konfigurira pravila sinkronizacije na:
  
- Koristite msDS-Konzistencyguid kao atribut sourceAnchor za korisničke objekte. ObjectGUID se koristi za druge vrste objekata.
    
- Za bilo koji određeni lokalni korisnički objekt oglasa čiji atribut msDS-Konzistencyguid nije popunjen, Azure AD Connect ponovno ispisuje vrijednost objectGUID-a na atribut MSD-Konzistencyguid u lokalno Active Directory. Nakon što se atribut msDS-Konzistencyguid popunjava, Azure AD Connect zatim izvozi objekt u Azure AD.
    
 **Napomena:** Kada se lokalni AD objekt uvozi u Azure AD Connect (koji se uvozi u prostor AD Connector i projicira u metaverse), više ne možete promijeniti svoju vrijednost sourceAnchor. Da biste odredili vrijednost sourceAnchor za određeni lokalno AD Object, konfigurirajte atribut MSD-Konzistencyguid prije nego što se uvozi u Azure AD Connect. 
  
Za više informacija o SourceAnchor i Konzistencyguid, pogledajte sljedeće: [Azure ad Connect: koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

