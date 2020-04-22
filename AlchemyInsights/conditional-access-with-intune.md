---
title: Uvjetni pristup s intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706013"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="b1d0b-102">Uvjetni pristup s intune</span><span class="sxs-lookup"><span data-stu-id="b1d0b-102">Conditional Access with Intune</span></span>

<span data-ttu-id="b1d0b-103">Korištenje **uvjetnog pristupa** s intuneom zahtijeva 3 koraka:</span><span class="sxs-lookup"><span data-stu-id="b1d0b-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="b1d0b-104">Stvorite **pravila uvjetnog pristupa** koja definiraju koji su resursi zaštićeni i koji su uvjeti potrebni za pristup tim resursima.</span><span class="sxs-lookup"><span data-stu-id="b1d0b-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="b1d0b-105">Na primjer, uređaj mora biti sukladan prije pristupanja korporativnoj e-pošti.</span><span class="sxs-lookup"><span data-stu-id="b1d0b-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="b1d0b-106">Stvorite **pravila usklađenosti** da biste definirali postavke koje se moraju ispuniti prije nego što se uređaj smatra sukladnim.</span><span class="sxs-lookup"><span data-stu-id="b1d0b-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="b1d0b-107">Na primjer, uređaj mora imati pin od najmanje 6 znamenki prije nego što se smatra sukladnim.</span><span class="sxs-lookup"><span data-stu-id="b1d0b-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="b1d0b-108">Osiguravanje **pravila usklađenosti** i **pravila uvjetnog pristupa** usmjerene su na željene grupe korisnika.</span><span class="sxs-lookup"><span data-stu-id="b1d0b-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="b1d0b-109">To može zahtijevati stvaranje određenih grupa korisnika u servisu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b1d0b-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="b1d0b-110">Opširnije::</span><span class="sxs-lookup"><span data-stu-id="b1d0b-110">Read more:</span></span>
  
- [<span data-ttu-id="b1d0b-111">Najbolji primjeri iz prakse za uvjetni pristup</span><span class="sxs-lookup"><span data-stu-id="b1d0b-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="b1d0b-112">Prvi koraci s uvjetnim pristupom</span><span class="sxs-lookup"><span data-stu-id="b1d0b-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

