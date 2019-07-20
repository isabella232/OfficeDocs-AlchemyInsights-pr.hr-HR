---
title: Nema rezultata pretraživanja sadržaja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800234"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="e9a63-102">Nema rezultata iz sadržaja pretraživanja/izvozi</span><span class="sxs-lookup"><span data-stu-id="e9a63-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="e9a63-103">Problemi s sadržaja pretraživanja/izvozi ne daje nikakve podatke možda određene usklađenosti sigurnost filtar koji je postavljanje određene Admin i nije je komunikacija sve administratori.</span><span class="sxs-lookup"><span data-stu-id="e9a63-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="e9a63-104">Da biste riješili taj problem, provjerite postoje filtre usklađenosti sigurnosti koji uzrokuje ovo:</span><span class="sxs-lookup"><span data-stu-id="e9a63-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="e9a63-105">Povezivanje s sigurnost i usklađenosti centar Powershell</span><span class="sxs-lookup"><span data-stu-id="e9a63-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="e9a63-106">Pokreni Cmdlete sljedeće:</span><span class="sxs-lookup"><span data-stu-id="e9a63-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="e9a63-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="e9a63-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="e9a63-108">Get-ComplianceSecurityFilter-$org organizacije</span><span class="sxs-lookup"><span data-stu-id="e9a63-108">Get-ComplianceSecurityFilter -Organization $org</span></span>