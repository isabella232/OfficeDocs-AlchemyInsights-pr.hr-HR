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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516965"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="5234d-102">ConsistencyGuid / sourceAnchor ponašanja</span><span class="sxs-lookup"><span data-stu-id="5234d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="5234d-103">Povezivanje Azure AD (verzija 1.1.524.0 i nakon) sada olakšava korištenje msDS ConsistencyGuid kao atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="5234d-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="5234d-104">Kada koristite tu značajku, Azure AD povezivanje automatski konfigurira pravila sinkronizacije:</span><span class="sxs-lookup"><span data-stu-id="5234d-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="5234d-105">Koristite msDS ConsistencyGuid kao atribut sourceAnchor za objekte korisnika.</span><span class="sxs-lookup"><span data-stu-id="5234d-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="5234d-106">ObjectGUID koristi se za druge vrste objekta.</span><span class="sxs-lookup"><span data-stu-id="5234d-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="5234d-107">Za bilo koju dali lokalno AD korisnik objekt čije msDS ConsistencyGuid atribut nije popunjen, Azure zapisivanja AD povezivanje njegova vrijednost objectGUID natrag na msDS ConsistencyGuid atribut u Active Directory lokalno.</span><span class="sxs-lookup"><span data-stu-id="5234d-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="5234d-108">Nakon popunjavaju msDS ConsistencyGuid atribut, Azure AD povezivanje Azure AD zatim izvozi objekt.</span><span class="sxs-lookup"><span data-stu-id="5234d-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="5234d-109">**Napomena:** Jednom se lokalno AD objekt uvoze Azure AD povezivanje (koja je, uvezeni u AD poveznik prostora i predviđena u u Metaverse), više ne možete promijeniti njegova vrijednost sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="5234d-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="5234d-110">Za određivanje vrijednosti sourceAnchor za u dao lokalno AD objekt, konfigurirajte njegov msDS ConsistencyGuid atribut prije je uvesti u Azure AD povezivanje.</span><span class="sxs-lookup"><span data-stu-id="5234d-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="5234d-111">Dodatne informacije o SourceAnchor i ConsistencyGuid, pogledajte sljedeće: [Azure AD povezivanje: dizajniranje koncepti](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="5234d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

