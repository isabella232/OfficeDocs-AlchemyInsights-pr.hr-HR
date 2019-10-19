---
title: Uvjetni pristup s Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36504986"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="aeb04-102">Uvjetni pristup s Intune</span><span class="sxs-lookup"><span data-stu-id="aeb04-102">Conditional Access with Intune</span></span>

<span data-ttu-id="aeb04-103">Korištenje **uvjetnog pristupa** s Intune zahtijeva 3 koraka:</span><span class="sxs-lookup"><span data-stu-id="aeb04-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="aeb04-104">Izradite **pravilnik o uvjetnom pristupu** koji definira koji se resursi štite i koje uvjete treba zadovoljiti da biste pristupili tim resursima.</span><span class="sxs-lookup"><span data-stu-id="aeb04-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="aeb04-105">Na primjer, uređaj mora biti usklađen prije pristupanja korporacijskoj e-pošti.</span><span class="sxs-lookup"><span data-stu-id="aeb04-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="aeb04-106">Stvorite **pravila usklađenosti** da biste definirali postavke koje moraju biti ispunjene prije nego što se uređaj smatra sukladnim.</span><span class="sxs-lookup"><span data-stu-id="aeb04-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="aeb04-107">Na primjer, uređaj mora imati PIN od najmanje 6 znamenki prije nego što se smatra sukladnim.</span><span class="sxs-lookup"><span data-stu-id="aeb04-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="aeb04-108">Osiguravanje **pravila usklađenosti** i pravila **uvjetnog pristupa** usmjerene su na željene grupe korisnika.</span><span class="sxs-lookup"><span data-stu-id="aeb04-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="aeb04-109">To može zahtijevati stvaranje određenih grupa korisnika u servisu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aeb04-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="aeb04-110">Pročitaj više:</span><span class="sxs-lookup"><span data-stu-id="aeb04-110">Read more:</span></span>
  
- [<span data-ttu-id="aeb04-111">Najbolje prakse uvjetnog pristupa</span><span class="sxs-lookup"><span data-stu-id="aeb04-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="aeb04-112">Početak početka s uvjetnim pristupom</span><span class="sxs-lookup"><span data-stu-id="aeb04-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

