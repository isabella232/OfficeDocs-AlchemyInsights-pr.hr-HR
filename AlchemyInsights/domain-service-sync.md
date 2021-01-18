---
title: Sinkronizacija servisa domene
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884844"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="2dfd7-102">Sinkronizacija servisa domene</span><span class="sxs-lookup"><span data-stu-id="2dfd7-102">Domain service synchronization</span></span>

<span data-ttu-id="2dfd7-103">Objekti i vjerodajnice u upravljanoj domeni servisa Azure Active Directory (Azure AD DS) mogu se stvarati lokalno unutar domene ili sinkronizirati iz korisnika Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2dfd7-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="2dfd7-104">Kada prvi put implementirate Azure AD DS, konfigurirajte jednosmjernu sinkronizaciju, a zatim pokrenete da biste replicirali objekte iz servisa Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2dfd7-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="2dfd7-105">Ovaj jednosmjerna sinkronizacija nastavlja se pokretati u pozadini da bi se u servisu Azure AD domogla ažurirane domene s promjenama iz Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2dfd7-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="2dfd7-106">Nema sinkronizacije iz servisa Azure AD DS natrag na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2dfd7-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="2dfd7-107">Dodatne informacije o sinkronizaciji servisa Azure Active Directory domena potražite u članku [Sinkronizacija servisa domene](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="2dfd7-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
