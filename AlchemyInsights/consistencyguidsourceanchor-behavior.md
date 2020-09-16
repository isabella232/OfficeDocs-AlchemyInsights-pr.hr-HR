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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="d1db1-102">Funkcija ConsistencyGuid/sourceanchor</span><span class="sxs-lookup"><span data-stu-id="d1db1-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="d1db1-103">Azure AD Connect (verzija 1.1.524.0 i nakon) sada olakšava korištenje servisa msDS-ConsistencyGuid kao atributa sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="d1db1-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="d1db1-104">Kada koristite ovu značajku, Azure AD Connect automatski konfigurira pravila sinkronizacije na sljedeće:</span><span class="sxs-lookup"><span data-stu-id="d1db1-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="d1db1-105">Koristite msDS-ConsistencyGuid kao atribut sourceAnchor za korisničke objekte.</span><span class="sxs-lookup"><span data-stu-id="d1db1-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="d1db1-106">ObjectGUID se koristi za druge vrste objekata.</span><span class="sxs-lookup"><span data-stu-id="d1db1-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="d1db1-107">Za bilo koji lokalni objekt oglasa za korisnike čiji atribut msDS-ConsistencyGuid nije popunjen, Azure AD Connect zapisuje vrijednost objectGUID natrag u atribut msDS-ConsistencyGuid u lokalnom servisu Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d1db1-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="d1db1-108">Kada se atribut msDS-ConsistencyGuid popunjava, Azure AD Connect zatim izvozi objekt na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d1db1-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="d1db1-109">**Upozorenje:** Kada se lokalni oglasni objekt uvozi u Azure AD Connect (to jest, uvezen u prostor OGLASNOG poveznika i projiciran na metaverse), više ne možete promijeniti vrijednost funkcije sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="d1db1-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="d1db1-110">Da biste naveli vrijednost sourceAnchor za navedeni lokalni objekt oglasa, konfigurirajte atribut msDS-ConsistencyGuid prije uvoza u Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d1db1-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="d1db1-111">Dodatne informacije o SourceAnchor i ConsistencyGuid-u potražite u sljedećim člancima: [Azure ad Connect: koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="d1db1-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

