---
title: Pokazatelji ne funkcioniraju pomoću preglednika Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676075"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="92b7d-102">Pokazatelji ne funkcioniraju pomoću preglednika Edge</span><span class="sxs-lookup"><span data-stu-id="92b7d-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="92b7d-103">Kada ste stvorili pokazatelj, edge ga ne poštuje (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="92b7d-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="92b7d-104">Dodatne informacije potražite u članku Stvaranje pokazatelja za IP adrese i [URL-ove/domene.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="92b7d-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="92b7d-105">1. korak: provjerite sljedeće</span><span class="sxs-lookup"><span data-stu-id="92b7d-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="92b7d-106">Provjerite je li pokazatelj točan (bez pogrešaka u IP/URL-u, ispravna radnja, ispravne RBAC grupe).</span><span class="sxs-lookup"><span data-stu-id="92b7d-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="92b7d-107">Pričekajte najmanje 2 sata nakon stvaranja pokazatelja da biste u obzir uzmu eventualnu latenciju.</span><span class="sxs-lookup"><span data-stu-id="92b7d-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="92b7d-108">Provjerite jesu li u programu Microsoft Defender za krajnju točku u sustavu Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="92b7d-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="92b7d-109">Provjerite mogu li ti sustavi komunicirati s oblakom.</span><span class="sxs-lookup"><span data-stu-id="92b7d-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="92b7d-110">Provjerite je li Smartscreen omogućen i dostupan tako da ode na [probno web-mjesto](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="92b7d-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="92b7d-111">Drugi korak: otklanjanje poteškoća s potencijalnim problemom</span><span class="sxs-lookup"><span data-stu-id="92b7d-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="92b7d-112">Provjerite zadovoljava li klijent preduvjete.</span><span class="sxs-lookup"><span data-stu-id="92b7d-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="92b7d-113">Detalje potražite u članku [Stvaranje pokazatelja za IP adrese i URL-ove/domene.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="92b7d-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="92b7d-114">Provjerite koristite li najnoviju verziju preglednika Edge.</span><span class="sxs-lookup"><span data-stu-id="92b7d-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="92b7d-115">Da biste saznali najnoviju verziju, pogledajte [u članku Saznajte koju verziju programa Microsoft Edge imate](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="92b7d-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="92b7d-116">Ponovno pokrenite preglednik Edge.</span><span class="sxs-lookup"><span data-stu-id="92b7d-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="92b7d-117">Pomaknite se do web-mjesta za koje imate pokazatelj postavljanja.</span><span class="sxs-lookup"><span data-stu-id="92b7d-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="92b7d-118">Ako se web-mjesto ne prikazuje očekivano, prijeđite na treći korak.</span><span class="sxs-lookup"><span data-stu-id="92b7d-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="92b7d-119">Treći korak: prikupljanje podataka</span><span class="sxs-lookup"><span data-stu-id="92b7d-119">Step 3: Collect data</span></span>

- <span data-ttu-id="92b7d-120">Prikupite **dijagnostičke podatke mdeclientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="92b7d-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="92b7d-121">Upute potražite u članku [Problemi s uređajem za unošenje na Microsoft Defender za krajnju točku](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="92b7d-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="92b7d-122">Ako ste zadovoljni instalacijom i prikupljanjem praćenja fiddlera, pogledajte [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="92b7d-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="92b7d-123">Ako želite smjernice Microsoftove podrške, odaberite ikonu Podrške u nastavku da biste otvorili slučaj podrške.</span><span class="sxs-lookup"><span data-stu-id="92b7d-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
