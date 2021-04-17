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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="ceea3-102">ConsistencyGuid / sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="ceea3-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="ceea3-103">Azure AD Connect (verzija 1.1.524.0 i nakon toga) sada olakšava korištenje atributa msDS-ConsistencyGuid kao atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="ceea3-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="ceea3-104">Kada koristite tu značajku, Azure AD Connect automatski konfigurira pravila sinkronizacije na sljedeće:</span><span class="sxs-lookup"><span data-stu-id="ceea3-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="ceea3-105">Koristite msDS-ConsistencyGuid kao atribut sourceAnchor za korisničke objekte.</span><span class="sxs-lookup"><span data-stu-id="ceea3-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="ceea3-106">ObjectGUID se koristi za druge vrste objekata.</span><span class="sxs-lookup"><span data-stu-id="ceea3-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="ceea3-107">Za bilo koji lokalni ad korisnički objekt čiji atribut msDS-ConsistencyGuid nije popunjen, Azure AD Connect vraća vrijednost objectGUID na atribut msDS-ConsistencyGuid u lokalnom servisu Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ceea3-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="ceea3-108">Kada se popunjava atribut msDS-ConsistencyGuid, Azure AD Connect zatim izvozi objekt u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ceea3-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="ceea3-109">**Napomena:** Kada se lokalni AD objekt uvozi u Azure AD Connect (to jest, uvozi se u prostor ad connectora i projiciran u Metaverse), više ne možete mijenjati njegovu izvornu vrijednostAnchor.</span><span class="sxs-lookup"><span data-stu-id="ceea3-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="ceea3-110">Da biste odredili vrijednost sourceAnchor za određeni lokalni AD objekt, prije uvoza u Azure AD Connect konfigurirajte atribut msDS-ConsistencyGuid.</span><span class="sxs-lookup"><span data-stu-id="ceea3-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="ceea3-111">Dodatne informacije o sourceAnchoru i dosljednostiGuid potražite u sljedećem: [Azure AD Connect: koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="ceea3-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

