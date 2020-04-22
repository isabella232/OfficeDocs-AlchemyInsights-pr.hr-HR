---
title: Praćenje uvjetnog pristupa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713710"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="bcbe8-102">Praćenje uvjetnog pristupa za Exchange</span><span class="sxs-lookup"><span data-stu-id="bcbe8-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="bcbe8-103">Korisnici koji ciljaju s uvjetnim pristupom primit će e-poruku s obavijesti ako ne ispunjavaju zahtjeve pristupa vaše tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="bcbe8-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="bcbe8-104">Da biste riješili problem, preporučujemo jedno ili više sljedećih rješenja:</span><span class="sxs-lookup"><span data-stu-id="bcbe8-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="bcbe8-105">Ako se pretpostavlja da je uređaj upisan, obavijestite korisnika da ode u aplikaciju Portal tvrtke i provjeri pojavljuje li se na portalu tvrtke.</span><span class="sxs-lookup"><span data-stu-id="bcbe8-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="bcbe8-106">Ako se to ne dogodi, korisnik bi trebao upisati uređaj.</span><span class="sxs-lookup"><span data-stu-id="bcbe8-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="bcbe8-107">Na portalu Azure idite na \*\*usklađenost uređaja Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="bcbe8-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="bcbe8-108">U **odjeljku Monitor** kliknite **Usklađenost uređaja**.</span><span class="sxs-lookup"><span data-stu-id="bcbe8-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="bcbe8-109">Pregledajte izvješće o usklađenosti uređaja da biste provjerili je li korisnikov uređaj označen kao sukladan.</span><span class="sxs-lookup"><span data-stu-id="bcbe8-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="bcbe8-110">Na portalu Azure idite na \*\*usklađenost uređaja Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="bcbe8-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="bcbe8-111">U **odjeljku Upravljanje**kliknite **Pravila**.</span><span class="sxs-lookup"><span data-stu-id="bcbe8-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="bcbe8-112">Na popisu pravila o usklađenosti provjerite je li profil dodijeljen uređaju vašeg korisnika.</span><span class="sxs-lookup"><span data-stu-id="bcbe8-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="bcbe8-113">Ako profil nije dodijeljen, Intune neće moći potvrditi status usklađenosti uređaja.</span><span class="sxs-lookup"><span data-stu-id="bcbe8-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="bcbe8-114">Uredite korisnikovu dodjelu uvjetnog pristupa.</span><span class="sxs-lookup"><span data-stu-id="bcbe8-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="bcbe8-115">Na portalu Azure idite na **Pravila uvjetnog pristupa \> \> Podešavanja**</span><span class="sxs-lookup"><span data-stu-id="bcbe8-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="bcbe8-116">Odabir pravila s popisa</span><span class="sxs-lookup"><span data-stu-id="bcbe8-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="bcbe8-117">Kliknite **Korisnici i grupe**</span><span class="sxs-lookup"><span data-stu-id="bcbe8-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="bcbe8-118">Da biste ciljali određena pravila kod nekoga, dodajte ih na popis **Uključi.**</span><span class="sxs-lookup"><span data-stu-id="bcbe8-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="bcbe8-119">Da biste osigurali da je osoba izostavljena iz pravila, dodajte je na popis **Izuzima.**</span><span class="sxs-lookup"><span data-stu-id="bcbe8-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="bcbe8-120">Opširnije: [Kako nadzirati uređaje uvjetnog pristupa](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="bcbe8-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

