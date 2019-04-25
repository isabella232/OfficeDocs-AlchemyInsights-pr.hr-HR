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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418461"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="da9fc-102">Nadzor uvjetno pristup</span><span class="sxs-lookup"><span data-stu-id="da9fc-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="da9fc-103">Ciljane uvjetno access korisnici će primiti obavijest e-pošte ako ne udovoljava zahtjevima pristupa vašoj organizaciji.</span><span class="sxs-lookup"><span data-stu-id="da9fc-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="da9fc-104">Da biste riješili, preporučujemo da jedno ili više od sljedećih rješenja:</span><span class="sxs-lookup"><span data-stu-id="da9fc-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="da9fc-105">Ako uređaj presumed da se upisani, savjeta korisnik Idi na Portal tvrtke app i provjerite pojavljuje se Portal tvrtke.</span><span class="sxs-lookup"><span data-stu-id="da9fc-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="da9fc-106">Ako ne, korisnik treba uvrstili uređaj.</span><span class="sxs-lookup"><span data-stu-id="da9fc-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="da9fc-107">Azure portal idite na **Intune \> usklađenosti uređaj**.</span><span class="sxs-lookup"><span data-stu-id="da9fc-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="da9fc-108">Ispod **monitora** kliknite **uređaj usklađenosti**.</span><span class="sxs-lookup"><span data-stu-id="da9fc-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="da9fc-109">Prikaz izvještaja usklađenosti uređaj da biste provjerili korisnički uređaj je označena kao sa standardom.</span><span class="sxs-lookup"><span data-stu-id="da9fc-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="da9fc-110">Azure portal idite na **Intune \> usklađenosti uređaj**.</span><span class="sxs-lookup"><span data-stu-id="da9fc-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="da9fc-111">U odjeljku **Upravljanje**kliknite **pravila**.</span><span class="sxs-lookup"><span data-stu-id="da9fc-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="da9fc-112">Na popisu pravila usklađenosti provjerite profil je dodijeljena svoj korisnički uređaj.</span><span class="sxs-lookup"><span data-stu-id="da9fc-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="da9fc-113">Ako je dodijeljen nijedan profil, zatim Intune nećete moći potvrditi statusom usklađenosti na uređaj.</span><span class="sxs-lookup"><span data-stu-id="da9fc-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="da9fc-114">Uređivanje korisnika uvjetno access dodjele.</span><span class="sxs-lookup"><span data-stu-id="da9fc-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="da9fc-115">Azure portal idite na **Intune \> uvjetno access \> pravila**</span><span class="sxs-lookup"><span data-stu-id="da9fc-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="da9fc-116">Odaberite pravilo s popisa</span><span class="sxs-lookup"><span data-stu-id="da9fc-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="da9fc-117">Kliknite **korisnici i grupe**</span><span class="sxs-lookup"><span data-stu-id="da9fc-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="da9fc-118">Ciljne određena pravila na netko, dodajte ih na popis za **Uvrštavanje** .</span><span class="sxs-lookup"><span data-stu-id="da9fc-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="da9fc-119">Da biste osigurali osoba izostavljen iz pravila, dodajte ih na popis za **izostavljanje** .</span><span class="sxs-lookup"><span data-stu-id="da9fc-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="da9fc-120">Pročitajte više: [Kako Access uvjetno Monitor uređaji](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="da9fc-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

