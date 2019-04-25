---
title: ConsistencyGuid / sourceAnchor ponašanja
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
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408100"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="535c5-102">ConsistencyGuid / sourceAnchor ponašanja</span><span class="sxs-lookup"><span data-stu-id="535c5-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="535c5-103">Povezivanje Azure AD (verzija 1.1.524.0 i nakon) sada olakšava korištenje msDS ConsistencyGuid kao atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="535c5-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="535c5-104">Kada koristite tu značajku, Azure AD povezivanje automatski konfigurira pravila sinkronizacije:</span><span class="sxs-lookup"><span data-stu-id="535c5-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="535c5-105">Koristite msDS ConsistencyGuid kao atribut sourceAnchor za objekte korisnika.</span><span class="sxs-lookup"><span data-stu-id="535c5-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="535c5-106">ObjectGUID koristi se za druge vrste objekta.</span><span class="sxs-lookup"><span data-stu-id="535c5-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="535c5-107">Za bilo koju dali lokalno AD korisnik objekt čije msDS ConsistencyGuid atribut nije popunjen, Azure zapisivanja AD povezivanje njegova vrijednost objectGUID natrag na msDS ConsistencyGuid atribut u Active Directory lokalno.</span><span class="sxs-lookup"><span data-stu-id="535c5-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="535c5-108">Nakon popunjavaju msDS ConsistencyGuid atribut, Azure AD povezivanje Azure AD zatim izvozi objekt.</span><span class="sxs-lookup"><span data-stu-id="535c5-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="535c5-109">**Napomena:** Jednom se lokalno AD objekt uvoze Azure AD povezivanje (koja je, uvezeni u AD poveznik prostora i predviđena u u Metaverse), više ne možete promijeniti njegova vrijednost sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="535c5-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="535c5-110">Za određivanje vrijednosti sourceAnchor za u dao lokalno AD objekt, konfigurirajte njegov msDS ConsistencyGuid atribut prije je uvesti u Azure AD povezivanje.</span><span class="sxs-lookup"><span data-stu-id="535c5-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="535c5-111">Dodatne informacije o SourceAnchor i ConsistencyGuid, pogledajte sljedeće: [Azure AD povezivanje: dizajniranje koncepti](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="535c5-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

