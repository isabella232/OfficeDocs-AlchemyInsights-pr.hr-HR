---
title: Uvjeti koje nema u trgovini termina sustava SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750443"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="f3168-102">Omogućivanje šifriranja BitLocker pomoću značajke Intune</span><span class="sxs-lookup"><span data-stu-id="f3168-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="f3168-103">Pravilnik o zaštiti krajnjih točaka može se koristiti za konfiguriranje postavki šifriranja za BitLocker za uređaje sa sustavom Windows, kao što je opisano u odjeljku: Windows10 (i novije) postavke za zaštitu uređaja pomoću aplikacije Intune</span><span class="sxs-lookup"><span data-stu-id="f3168-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="f3168-104">Morate biti svjesni da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko šifriranje šifriranja koje se pokreće bez primjene pravilnika MDM-a.</span><span class="sxs-lookup"><span data-stu-id="f3168-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="f3168-105">To može utjecati na primjenu Pravilnika ako su konfigurirane standardne postavke.</span><span class="sxs-lookup"><span data-stu-id="f3168-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="f3168-106">Dodatne pojedinosti potražite u članku Najčešća pitanja.</span><span class="sxs-lookup"><span data-stu-id="f3168-106">See FAQ for more detail.</span></span>


<span data-ttu-id="f3168-107">FAQ   Q: koja izdanja sustava Windows podržava šifriranje uređaja pomoću pravilnika o zaštiti krajnjih točaka?</span><span class="sxs-lookup"><span data-stu-id="f3168-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="f3168-108"> A: postavke u pravilu zaštite krajnjih točaka implementiraju se pomoću značajke BitLocker CSP-a.</span><span class="sxs-lookup"><span data-stu-id="f3168-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="f3168-109">Ne podržavaju sva izdanja ni verzije sustava Windows pomoću značajke BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="f3168-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="f3168-110">U ovom trenutku izdanja sustava Windows: Enterprise; Podržani su edukacijski, mobilni, mobilni Enterprise i Professional (od međuverzija 1809 prema dalje).</span><span class="sxs-lookup"><span data-stu-id="f3168-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="f3168-111">P: ako je uređaj već šifriran uz BitLocker pomoću zadanih postavki OS-a za metodu šifriranja i čvrstoću šifriranja (XTT-AIS-128) primjenjuje pravilo s drugim postavkama automatski pokreće ponovnu šifriranje pogona pomoću novih postavki?</span><span class="sxs-lookup"><span data-stu-id="f3168-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="f3168-112">O: Ne.</span><span class="sxs-lookup"><span data-stu-id="f3168-112">A: No.</span></span> <span data-ttu-id="f3168-113">Da bi se primijenile nove postavke šifre, pogon mora prvo biti dešifriran.</span><span class="sxs-lookup"><span data-stu-id="f3168-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="f3168-114">Podsjetnik za uređaje koji se upisuju uz autopilot automatsko šifriranje koje se događa tijekom programa OOBE nije pokrenuto dok se ne procjenjuje pravilo Intune koja omogućuje postavljanje postavki pravilnika koje se koriste umjesto zadanih vrijednosti OS-a.</span><span class="sxs-lookup"><span data-stu-id="f3168-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="f3168-115">Q ako je uređaj šifriran kao rezultat primjene pravilnika za Intune, hoće li se dešifrirati kada se to pravilo Ukloni?</span><span class="sxs-lookup"><span data-stu-id="f3168-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="f3168-116">O: uklanjanje šifriranja povezanog pravilnika ne rezultira dešifriranjem diskova koji su konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="f3168-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="f3168-117">P: Zašto pravilnik o pridržavanju sukladnosti pokazuje da moj uređaj nema "omogućen BitLocker", ali jest?</span><span class="sxs-lookup"><span data-stu-id="f3168-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="f3168-118">A: postavka "omogućeno BitLocker" u pravilima za usklađenost s usklađenosti koristi klijent za zdravlje servisa Windows Device (ĐD).</span><span class="sxs-lookup"><span data-stu-id="f3168-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="f3168-119">Ovaj klijent samo mjeri stanje uređaja u vremenu dizanja.</span><span class="sxs-lookup"><span data-stu-id="f3168-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="f3168-120">Dakle, ako uređaj nije ponovno pokrenuto budući da je BitLocker enkripcija dovršen, servis za klijentski softver u programu ĐHA neće prijaviti BitLocker kao aktivan.</span><span class="sxs-lookup"><span data-stu-id="f3168-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>