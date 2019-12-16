---
title: Uvjeti koji nedostaju iz spremišta termina SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053505"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="19731-102">Omogućavanje BitLocker šifriranja s Intune</span><span class="sxs-lookup"><span data-stu-id="19731-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="19731-103">Intune pravilo zaštite sigurnosti može se koristiti za konfiguriranje postavke šifriranja Boitlocker za Windows uređaje kao što je opisano u: Windows10 (i noviji) postavke za zaštitu uređaja pomoću Intune</span><span class="sxs-lookup"><span data-stu-id="19731-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="19731-104">Trebali biste biti svjesni da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko BitLocker šifriranje koje se aktivira bez primjene MDM pravila.</span><span class="sxs-lookup"><span data-stu-id="19731-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="19731-105">To može utjecati na primjenu pravila ako su konfigurirane nezadane postavke.</span><span class="sxs-lookup"><span data-stu-id="19731-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="19731-106">Pogledajte FAQ za više detalja.</span><span class="sxs-lookup"><span data-stu-id="19731-106">See FAQ for more detail.</span></span>


<span data-ttu-id="19731-107">Često  postavljana pitanja Q: koja izdanja sustava Windows podržavaju šifriranje uređaja pomoću pravila o zaštiti krajnjih točaka?</span><span class="sxs-lookup"><span data-stu-id="19731-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="19731-108"> O: postavke u pravilima zaštite sigurnosti Intune provode se pomoću BitLocker CSP-a.</span><span class="sxs-lookup"><span data-stu-id="19731-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="19731-109">Ne podržavaju sva izdanja ni verzije sustava Windows BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="19731-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="19731-110">U ovom trenutku izdanja sustava Windows: Enterprise; Podržano je obrazovanje, Mobilno, Mobilno poduzeće i profesionalni (od izgradnje 1809 prema naprijed).</span><span class="sxs-lookup"><span data-stu-id="19731-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="19731-111">P: ako je uređaj već šifriran s BitLocker pomoću zadane postavke OS-a za metodu šifriranja i čvrstoću šifriranje (XTS-AES-128) će primijeniti pravilo s različitim postavkama automatski aktivirati ponovno šifriranje pogona s novim postavkama?</span><span class="sxs-lookup"><span data-stu-id="19731-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="19731-112">A: ne.</span><span class="sxs-lookup"><span data-stu-id="19731-112">A: No.</span></span> <span data-ttu-id="19731-113">Kako biste primijenili nove postavke šifriranja, pogon mora prvo biti dešifriran.</span><span class="sxs-lookup"><span data-stu-id="19731-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="19731-114">Napomena za uređaje koji se upisuje autopilotom automatsko šifriranje koje će se pojaviti tijekom OOBE ne pokreće se dok se ne ocijeni pravila Intune koja omogućuje postavljanje postavki utemeljenih na pravilima za zadane postavke operacijskog sustava</span><span class="sxs-lookup"><span data-stu-id="19731-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="19731-115">Q ako je uređaj šifriran kao rezultat primjene pravila Intune hoće li se dešifrirati kada se ta pravila uklone?</span><span class="sxs-lookup"><span data-stu-id="19731-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="19731-116">O: uklanjanje pravila povezanih s šifriranjem ne rezultira dekriptiranje diskova koji su konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="19731-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="19731-117">P: Zašto neprecizno pravilo usklađenosti pokazuje da moj uređaj nema "BitLocker omogućen", ali je?</span><span class="sxs-lookup"><span data-stu-id="19731-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="19731-118">A: postavka "omogućeno za BitLocker" u pravilima usklađenosti koristi se s klijentskim programom za osiguranje sustava Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="19731-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="19731-119">Ovaj klijent mjeri stanje uređaja samo u vrijeme pokretanja.</span><span class="sxs-lookup"><span data-stu-id="19731-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="19731-120">Dakle, ako se uređaj nije ponovno pokrenuo jer je BitLocker šifriranje dovršen, usluga DHA klijenta neće prijaviti BitLocker kao aktivnu.</span><span class="sxs-lookup"><span data-stu-id="19731-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>