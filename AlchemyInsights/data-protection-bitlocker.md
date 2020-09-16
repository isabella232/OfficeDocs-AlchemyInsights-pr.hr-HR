---
title: Zaštita podataka – BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731231"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="df376-102">Omogućivanje šifriranja BitLocker pomoću značajke Intune</span><span class="sxs-lookup"><span data-stu-id="df376-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="df376-103">Pravilnik o zaštiti krajnjih točaka može se koristiti za konfiguriranje postavki šifriranja BitLocker za uređaje sa sustavom Windows.</span><span class="sxs-lookup"><span data-stu-id="df376-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="df376-104">Dodatne informacije potražite u članku [Postavke sustava Windows 10 (i novije) radi zaštite uređaja pomoću značajke Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="df376-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="df376-105">Morate biti svjesni da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko šifriranje BitLocker šifriranja, koji se pokreće bez primjene pravilnika MDM-a.</span><span class="sxs-lookup"><span data-stu-id="df376-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="df376-106">To može utjecati na primjenu Pravilnika ako su konfigurirane postavke koje nisu zadane.</span><span class="sxs-lookup"><span data-stu-id="df376-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="df376-107">Dodatne pojedinosti potražite u sljedećim najčešća pitanja.</span><span class="sxs-lookup"><span data-stu-id="df376-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="df376-108">Informacije o otklanjanju poteškoća sa značajkom BitLocker potražite [u članku Otklanjanje poteškoća s značajkom BitLocker u programu Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="df376-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="df376-109">**Najčešća pitanja**</span><span class="sxs-lookup"><span data-stu-id="df376-109">**FAQ**</span></span>

 <span data-ttu-id="df376-110">P: koja izdanja sustava Windows podržava šifriranje uređaja pomoću pravilnika o zaštiti krajnjih točaka?</span><span class="sxs-lookup"><span data-stu-id="df376-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="df376-111">A: postavke u pravilu zaštite krajnjih točaka implementiraju se pomoću [značajke BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)-a.</span><span class="sxs-lookup"><span data-stu-id="df376-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="df376-112">Ne podržavaju sva izdanja ili verzije sustava Windows pomoću značajke BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="df376-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="df376-113">U ovom se trenutku podržavaju sljedeća izdanja sustava Windows: Enterprise, Education, Mobile, Mobile Enterprise i Professional (međuverzija 1809 i noviji).</span><span class="sxs-lookup"><span data-stu-id="df376-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="df376-114">P: ako je uređaj već šifriran uz BitLocker pomoću zadanih postavki OS-a za metodu šifriranja i čvrstoću šifriranja (XTT-AIS-128), hoće li primjena pravilnika s drugim postavkama automatski aktivirati ponovno šifriranje pogona pomoću novih postavki?</span><span class="sxs-lookup"><span data-stu-id="df376-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="df376-115">O: Ne.</span><span class="sxs-lookup"><span data-stu-id="df376-115">A: No.</span></span> <span data-ttu-id="df376-116">Da biste primijenili nove postavke šifriranja, pogon mora prvo biti dešifriran.</span><span class="sxs-lookup"><span data-stu-id="df376-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="df376-117">**Upozorenje:** Da bi se uređaji upisali kao autopilot, automatsko šifriranje koje bi se dogodilo tijekom programa OOBE ne pokreće se dok se ne procjenjuje pravilo Intune, što omogućuje postavljanje postavki temeljenih na pravilima na mjestu zadane vrijednosti OS-a.</span><span class="sxs-lookup"><span data-stu-id="df376-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="df376-118">P: ako je uređaj šifriran kao rezultat aplikacije Intune Policy, hoće li se dešifrirati kada se to pravilo Ukloni?</span><span class="sxs-lookup"><span data-stu-id="df376-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="df376-119">A: uklanjanje pravilnika koje se odnose na šifriranje ne rezultira dešifriranjem diskova koji su konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="df376-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="df376-120">P: Zašto pravilnik o pridržavanju sukladnosti pokazuje da moj uređaj nema omogućen BitLocker, čak i ako jest?</span><span class="sxs-lookup"><span data-stu-id="df376-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="df376-121">A: postavka "omogućeno BitLocker" u politici usklađivanja usklađenosti koristi klijent sustava Windows za zdravlje attestation (ĐD).</span><span class="sxs-lookup"><span data-stu-id="df376-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="df376-122">Ovaj klijent samo mjeri stanje uređaja u vremenu dizanja.</span><span class="sxs-lookup"><span data-stu-id="df376-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="df376-123">Dakle, ako uređaj nije ponovno pokrenuto nakon dovršetka šifriranja BitLocker, servis servisa ĐHA Client neće prijaviti BitLocker kao aktivan.</span><span class="sxs-lookup"><span data-stu-id="df376-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 