---
title: Nema rezultata pretraživanja sadržaja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680639"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="14660-102">Nema rezultata pretraživanja sadržaja/izvoza</span><span class="sxs-lookup"><span data-stu-id="14660-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="14660-103">Problemi s pretraživanjem sadržaja/izvozom koji ne vraća podatke možda je razlog za određeni sigurnosni filtar za usklađenost koji je postavio određeni administrator i nije ga mogao komunicirati sa svim administratorima.</span><span class="sxs-lookup"><span data-stu-id="14660-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="14660-104">Da biste riješili taj problem, provjerite postoje li neki sigurnosni filtri za usklađenost koji mogu prouzročiti sljedeće:</span><span class="sxs-lookup"><span data-stu-id="14660-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="14660-105">Spojite se na PowerShell centra za sigurnost i usklađenost</span><span class="sxs-lookup"><span data-stu-id="14660-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="14660-106">Pokrenite sljedeće cmdlets:</span><span class="sxs-lookup"><span data-stu-id="14660-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="14660-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="14660-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="14660-108">Filtar za dohvaćanje i usklađenost $org</span><span class="sxs-lookup"><span data-stu-id="14660-108">Get-ComplianceSecurityFilter -Organization $org</span></span>