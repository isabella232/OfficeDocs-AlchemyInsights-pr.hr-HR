---
title: Nadzor uvjetno pristup
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902333"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="0e3bf-102">Nadzor uvjetno pristup</span><span class="sxs-lookup"><span data-stu-id="0e3bf-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="0e3bf-p101">Ciljane uvjetno access korisnici će primiti obavijest e-pošte ako ne udovoljava zahtjevima pristupa vašoj organizaciji. Da biste riješili, preporučujemo da jedno ili više od sljedećih rješenja:</span><span class="sxs-lookup"><span data-stu-id="0e3bf-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="0e3bf-p102">Ako uređaj presumed da se upisani, savjeta korisnik Idi na Portal tvrtke app i provjerite pojavljuje se Portal tvrtke. Ako ne, korisnik treba uvrstili uređaj.</span><span class="sxs-lookup"><span data-stu-id="0e3bf-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="0e3bf-p103">Azure portal idite na **Intune \> usklađenosti uređaj**. Ispod **monitora** kliknite **uređaj usklađenosti**. Prikaz izvještaja usklađenosti uređaj da biste provjerili korisnički uređaj je označena kao sa standardom.</span><span class="sxs-lookup"><span data-stu-id="0e3bf-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="0e3bf-p104">Azure portal idite na **Intune \> usklađenosti uređaj**. U odjeljku **Upravljanje**kliknite **pravila**. Na popisu pravila usklađenosti provjerite profil je dodijeljena svoj korisnički uređaj. Ako je dodijeljen nijedan profil, zatim Intune nećete moći potvrditi statusom usklađenosti na uređaj.</span><span class="sxs-lookup"><span data-stu-id="0e3bf-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="0e3bf-114">Uređivanje korisnika uvjetno access dodjele.</span><span class="sxs-lookup"><span data-stu-id="0e3bf-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="0e3bf-115">Azure portal idite na **Intune \> uvjetno access \> pravila**</span><span class="sxs-lookup"><span data-stu-id="0e3bf-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="0e3bf-116">Odaberite pravilo s popisa</span><span class="sxs-lookup"><span data-stu-id="0e3bf-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="0e3bf-117">Kliknite **korisnici i grupe**</span><span class="sxs-lookup"><span data-stu-id="0e3bf-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="0e3bf-p105">Ciljne određena pravila na netko, dodajte ih na popis za **Uvrštavanje** . Da biste osigurali osoba izostavljen iz pravila, dodajte ih na popis za **izostavljanje** .</span><span class="sxs-lookup"><span data-stu-id="0e3bf-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="0e3bf-120">Pročitajte više: [Kako Access uvjetno Monitor uređaji](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="0e3bf-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

