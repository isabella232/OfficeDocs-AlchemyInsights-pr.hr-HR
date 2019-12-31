---
title: Data Protection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908702"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="7e1d5-102">Omogućavanje BitLocker šifriranja s Intune</span><span class="sxs-lookup"><span data-stu-id="7e1d5-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="7e1d5-103">Intune pravila o zaštiti krajnjih točaka mogu se koristiti za konfiguriranje postavki BitLocker šifriranja za uređaje sa sustavom Windows.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="7e1d5-104">Dodatne informacije potražite u odjeljku [Postavke sustava Windows 10 (i noviji) kako biste zaštitili uređaje pomoću programa Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="7e1d5-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="7e1d5-105">Trebali biste biti svjesni da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko BitLocker šifriranje, koje se aktivira bez primjene MDM pravila.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="7e1d5-106">To može utjecati na primjenu pravila ako su konfigurirane postavke koje nisu zadane.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="7e1d5-107">Dodatne pojedinosti potražite u sljedećim FAQ-u.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="7e1d5-108">Informacije o rješavanju problema s BitLocker podacima potražite [u članku Otklanjanje poteškoća s BitLocker pravilima u programu Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="7e1d5-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="7e1d5-109">**Faq**</span><span class="sxs-lookup"><span data-stu-id="7e1d5-109">**FAQ**</span></span>

 <span data-ttu-id="7e1d5-110">P: koja izdanja sustava Windows podržavaju šifriranje uređaja pomoću pravila za zaštitu krajnjih točaka?</span><span class="sxs-lookup"><span data-stu-id="7e1d5-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="7e1d5-111">O: postavke u pravilima o zaštiti krajnjih točaka Intune provode se pomoću [BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)-a.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="7e1d5-112">Ne podržavaju sva izdanja ili verzije sustava Windows BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="7e1d5-113">U ovom trenutku podržane su sljedeće izdanja sustava Windows: Enterprise, Education, Mobile, Mobile Enterprise i Professional (Build 1809 i noviji).</span><span class="sxs-lookup"><span data-stu-id="7e1d5-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="7e1d5-114">P: ako je uređaj već šifriran s BitLocker pomoću zadane postavke OS-a za metodu šifriranja i snagu šifriranja (XTS-AES-128), primijenit će pravila s različitim postavkama automatski aktivirati ponovno šifriranje pogona novim postavkama?</span><span class="sxs-lookup"><span data-stu-id="7e1d5-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="7e1d5-115">A: ne.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-115">A: No.</span></span> <span data-ttu-id="7e1d5-116">Da biste primijenili nove postavke šifriranja, pogon prvo mora biti dešifriran.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="7e1d5-117">**Napomena:** Za uređaje koji se upisuje autopilot, automatsko šifriranje koje će se pojaviti tijekom OOBE-a ne aktivira se dok se ne ocijeni pravila Intune, što omogućuje da se postavke temeljene na politici koriste umjesto zadanih postavki operacijskog sustava.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="7e1d5-118">P: ako je uređaj šifriran zbog primjene pravila Intune, hoće li se dešifrirati kada se ta pravila uklone?</span><span class="sxs-lookup"><span data-stu-id="7e1d5-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="7e1d5-119">A: uklanjanje pravila vezanih za šifriranje ne rezultira dešifriranjem diskova koji su konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="7e1d5-120">P: Zašto pravila o sukladnosti Intune pokazuju da moj uređaj nije omogućen za BitLocker, iako je to?</span><span class="sxs-lookup"><span data-stu-id="7e1d5-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="7e1d5-121">A: postavka "omogućena za BitLocker" u politici sukladnosti sustava pravilne uporabe koristi klijent za zdravlje uređaja za zdravstvenu potvrdu (DHA).</span><span class="sxs-lookup"><span data-stu-id="7e1d5-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="7e1d5-122">Ovaj klijent mjeri stanje uređaja samo u vrijeme pokretanja.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="7e1d5-123">Dakle, ako se uređaj nije ponovno pokrenuo od dovršetka BitLocker šifriranja, usluga DHA klijenta neće prijaviti BitLocker kao aktivnu.</span><span class="sxs-lookup"><span data-stu-id="7e1d5-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 