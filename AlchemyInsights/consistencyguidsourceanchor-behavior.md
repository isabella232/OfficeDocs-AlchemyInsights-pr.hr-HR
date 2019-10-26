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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="4a713-102">Ponašanje za Konzistenceguid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="4a713-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="4a713-103">Azure AD Connect (verzija 1.1.524.0 i after) sada olakšava korištenje atributa msDS-</span><span class="sxs-lookup"><span data-stu-id="4a713-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="4a713-104">Kada koristite ovu značajku, Azure AD Connect automatski konfigurira pravila sinkronizacije na:</span><span class="sxs-lookup"><span data-stu-id="4a713-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="4a713-105">Koristite msDS-Konzistencyguid kao atribut sourceAnchor za korisničke objekte.</span><span class="sxs-lookup"><span data-stu-id="4a713-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="4a713-106">ObjectGUID se koristi za druge vrste objekata.</span><span class="sxs-lookup"><span data-stu-id="4a713-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="4a713-107">Za bilo koji određeni lokalni korisnički objekt oglasa čiji atribut msDS-Konzistencyguid nije popunjen, Azure AD Connect ponovno ispisuje vrijednost objectGUID-a na atribut MSD-Konzistencyguid u lokalno Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4a713-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="4a713-108">Nakon što se atribut msDS-Konzistencyguid popunjava, Azure AD Connect zatim izvozi objekt u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a713-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="4a713-109">**Napomena:** Kada se lokalni AD objekt uvozi u Azure AD Connect (koji se uvozi u prostor AD Connector i projicira u metaverse), više ne možete promijeniti svoju vrijednost sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="4a713-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="4a713-110">Da biste odredili vrijednost sourceAnchor za određeni lokalno AD Object, konfigurirajte atribut MSD-Konzistencyguid prije nego što se uvozi u Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="4a713-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="4a713-111">Za više informacija o SourceAnchor i Konzistencyguid, pogledajte sljedeće: [Azure ad Connect: koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="4a713-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

