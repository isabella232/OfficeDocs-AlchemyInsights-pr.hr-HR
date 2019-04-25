---
title: Uvjetno Access s Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393533"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="53b62-102">Uvjetno Access s Intune</span><span class="sxs-lookup"><span data-stu-id="53b62-102">Conditional Access with Intune</span></span>

<span data-ttu-id="53b62-103">Pomoću **Uvjetnog Access** s Intune zahtijeva korake 3:</span><span class="sxs-lookup"><span data-stu-id="53b62-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="53b62-104">Stvaranje **Pravila uvjetnog pristup** koji definira zaštićeni su resursima i što uvjete treba zadovoljiti pristup tih resursa.</span><span class="sxs-lookup"><span data-stu-id="53b62-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="53b62-105">Ako, na primjer, uređaj mora biti usklađen prije pristupanja tvrtke e-pošte.</span><span class="sxs-lookup"><span data-stu-id="53b62-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="53b62-106">Stvaranje **Pravila usklađenosti** definirati postavke koje treba zadovoljiti prije smatra se uređaj sa standardom.</span><span class="sxs-lookup"><span data-stu-id="53b62-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="53b62-107">Ako, na primjer, uređaj mora imati pin barem 6 znamenke prije smatra se sa standardom.</span><span class="sxs-lookup"><span data-stu-id="53b62-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="53b62-108">Osiguravanje **Pravila usklađenosti** i **Pravilima uvjetnog Access** ciljan za željeni grupe korisnika.</span><span class="sxs-lookup"><span data-stu-id="53b62-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="53b62-109">To može zahtijevati stvaranje određene grupe korisnika Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="53b62-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="53b62-110">Pročitajte više:</span><span class="sxs-lookup"><span data-stu-id="53b62-110">Read more:</span></span>
  
- [<span data-ttu-id="53b62-111">Uvjetno Access Najbolji postupci</span><span class="sxs-lookup"><span data-stu-id="53b62-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="53b62-112">Uvod uvjetno Access</span><span class="sxs-lookup"><span data-stu-id="53b62-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

