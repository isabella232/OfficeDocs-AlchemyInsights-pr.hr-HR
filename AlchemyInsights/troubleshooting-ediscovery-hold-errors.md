---
title: Otklanjanje poteškoća s otkrivanjem e-otkrivanja zadržava pogreške
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676051"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="2761b-102">Otklanjanje poteškoća s otkrivanjem e-otkrivanja zadržava pogreške</span><span class="sxs-lookup"><span data-stu-id="2761b-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="2761b-103">Nailazite na probleme s čuvanjem predočavanja elektroničkih elektroničkih elektroničkih podataka?</span><span class="sxs-lookup"><span data-stu-id="2761b-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="2761b-104">Evo nekoliko najboljih praksi koje možete uzeti u obzir:</span><span class="sxs-lookup"><span data-stu-id="2761b-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="2761b-105">Provjerite stanje raspodjele čekanja.</span><span class="sxs-lookup"><span data-stu-id="2761b-105">Check the hold distribution status.</span></span>  <span data-ttu-id="2761b-106">Ako je status **Na čekanju ili** **Isključeno (na čekanju),** pričekajte da se raspodjela čekanja dovrši.</span><span class="sxs-lookup"><span data-stu-id="2761b-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="2761b-107">Spoji eDiscovery zadržava ažuriranja u jedan skupni zahtjev umjesto da se pravilnik neprestano ažurira za svaku transakciju.</span><span class="sxs-lookup"><span data-stu-id="2761b-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="2761b-108">Pokrenite Set-CaseHoldPolicy <policyname> -RetryDistribution u ljuski Powershell centra za sigurnost i usklađenost.</span><span class="sxs-lookup"><span data-stu-id="2761b-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="2761b-109">Detalje potražite u [članku Povezivanje komponente PowerShell & sigurnosti](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="2761b-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="2761b-110">Upute za provjeru tih postavki i dodatnih najboljih praksi za ublažavanje i rješavanje predočavanja elektroničkih elektroničkih podataka potražite u članku Otklanjanje pogrešaka prilikom čuvanja elektroničkih elektroničkih [podataka](/microsoft-365/compliance/hold-distribution-errors).</span><span class="sxs-lookup"><span data-stu-id="2761b-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="2761b-111">Informacije o otklanjanju poteškoća s drugim uobičajenim problemima predočavanja elektroničkih elektroničkih podataka potražite u članku Istraživanje, otklanjanje poteškoća i rješavanje uobičajenih problema [s predočavanje elektroničkih podataka](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span><span class="sxs-lookup"><span data-stu-id="2761b-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
