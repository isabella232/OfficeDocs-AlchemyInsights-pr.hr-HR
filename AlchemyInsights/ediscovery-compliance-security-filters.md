---
title: Nema povratnih rezultata tijekom pretraživanja sadržaja/izvoza
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727215"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="13c39-102">Nema povratnih rezultata tijekom pretraživanja sadržaja/izvoza</span><span class="sxs-lookup"><span data-stu-id="13c39-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="13c39-103">Ako nailazite na probleme s sljedećim scenarijima za otkrivanje:</span><span class="sxs-lookup"><span data-stu-id="13c39-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="13c39-104">Pretraživanje sadržaja/izvoz ne vraća nikakve podatke ni neočekivane podatke</span><span class="sxs-lookup"><span data-stu-id="13c39-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="13c39-105">Pretraživanje ili izvoz razotkrivanja nije uspjelo</span><span class="sxs-lookup"><span data-stu-id="13c39-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="13c39-106">Možda se radi o određenim sigurnosnim filtrima za usklađenost koje je postavljen određeni administrator, a nisu priopćeni svim administratorima.</span><span class="sxs-lookup"><span data-stu-id="13c39-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="13c39-107">Da biste riješili taj problem, provjerite postoje li sigurnosni filtri za usklađenost koji mogu uzrokovati te probleme:</span><span class="sxs-lookup"><span data-stu-id="13c39-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="13c39-108">Spojite se na PowerShell centra za sigurnost i usklađenost</span><span class="sxs-lookup"><span data-stu-id="13c39-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="13c39-109">Pokrenite sljedeće cmdlets:</span><span class="sxs-lookup"><span data-stu-id="13c39-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="13c39-110">Dodatne informacije o sigurnosnim filtrima usklađenosti potražite u članku [Filtriranje dozvola za pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="13c39-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
