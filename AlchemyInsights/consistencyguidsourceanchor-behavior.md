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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="f6ae3-102">Ponašanje DosljednostGuid / sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="f6ae3-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="f6ae3-103">Azure AD Connect (verzija 1.1.524.0 i nakon) sada olakšava korištenje msDS-DosljednostGuid kao atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="f6ae3-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="f6ae3-104">Kada koristite ovu značajku, Azure AD Connect automatski konfigurira pravila sinkronizacije na:</span><span class="sxs-lookup"><span data-stu-id="f6ae3-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="f6ae3-105">Koristite msDS-DosljednostGuid kao atribut sourceAnchor za korisničke objekte.</span><span class="sxs-lookup"><span data-stu-id="f6ae3-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="f6ae3-106">ObjectGUID se koristi za druge vrste objekata.</span><span class="sxs-lookup"><span data-stu-id="f6ae3-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="f6ae3-107">Za sve dane lokalni objekt AD Korisnik čiji atribut msDS-DosljednostGuid nije popunjen, Azure AD Connect vraća svoju vrijednost objectGUID natrag na atribut msDS-DosljednostGuid u lokalnom servisu Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f6ae3-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="f6ae3-108">Nakon popunjavanja atributa msDS-DosljednostGuid, Azure AD Connect zatim izvozi objekt u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f6ae3-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="f6ae3-109">**Napomena:** Nakon što se lokalni AD objekt uveze u Azure AD Connect (tj. uvozi u prostor AD poveznika i projicira u Metaverse), više ne možete promijeniti njegovu vrijednost sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="f6ae3-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="f6ae3-110">Da biste odredili vrijednost sourceAnchor za određeni lokalni AD objekt, konfigurirajte njegov atribut msDS-DosljednostGuid prije uvoza u Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f6ae3-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="f6ae3-111">Dodatne informacije o SourceAnchor i DosljednostGuid potražite u sljedećim [člancima Azure AD Connect: Koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="f6ae3-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

