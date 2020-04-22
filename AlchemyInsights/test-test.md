---
title: Pojmovi koji nedostaju u spremištu termina sustava SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766845"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="d600f-102">Omogućavanje Bitlocker šifriranja pomoću intune</span><span class="sxs-lookup"><span data-stu-id="d600f-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="d600f-103">Intune Endpoint Protection Policy može se koristiti za konfiguriranje BoitLocker postavki šifriranja za Windows uređaje kao što je opisano u : Postavke sustava Windows10 (i noviji) za zaštitu uređaja pomoću intune</span><span class="sxs-lookup"><span data-stu-id="d600f-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="d600f-104">Trebali biste biti svjesni da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko bitlocker šifriranje koje se pokreće bez primjene MDM pravila.</span><span class="sxs-lookup"><span data-stu-id="d600f-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="d600f-105">To može utjecati na primjenu pravila ako su konfigurirane postavke koje nisu zadane.</span><span class="sxs-lookup"><span data-stu-id="d600f-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="d600f-106">Pogledajte najčešća pitanja za više detalja.</span><span class="sxs-lookup"><span data-stu-id="d600f-106">See FAQ for more detail.</span></span>


<span data-ttu-id="d600f-107">Faq  P: Koja izdanja sustava Windows podržavaju šifriranje uređaja pomoću pravila zaštite krajnje točke?</span><span class="sxs-lookup"><span data-stu-id="d600f-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="d600f-108"> O: Postavke u pravilima zaštite krajnje točke intune implementiraju se pomoću Bitlocker CSP-a.</span><span class="sxs-lookup"><span data-stu-id="d600f-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="d600f-109">Ne podržavaju sva izdanja ni međuverzije sustava Windows Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="d600f-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="d600f-110">U ovom trenutku Windows Izdanja: Enterprise; Obrazovanje, Koji se kreće, Koji se kreće Poduzeće i Koji se odnosi na zvanje ( from graditi 1809 nadalje) jesu podržanih od.</span><span class="sxs-lookup"><span data-stu-id="d600f-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="d600f-111">P: Ako je uređaj već šifriran s BitLocker pomoću zadanih postavki OS-a za metodu šifriranja i snagu šifriranja (XTS-AES-128) će primijeniti pravila s različitim postavkama automatski će pokrenuti ponovno šifriranje pogona s novim postavkama?</span><span class="sxs-lookup"><span data-stu-id="d600f-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="d600f-112">A: Ne.</span><span class="sxs-lookup"><span data-stu-id="d600f-112">A: No.</span></span> <span data-ttu-id="d600f-113">Da biste primijenili nove postavke šifriranja, pogon se najprije mora dešifrirati.</span><span class="sxs-lookup"><span data-stu-id="d600f-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="d600f-114">Napomena Za uređaje koji se upisuju s autopilotom automatsko šifriranje koje će se dogoditi tijekom oOBE-a ne pokreće se dok se ne procijeni intune pravilo koje omogućuje da se umjesto zadanih postavki osustavu OS koriste postavke utemeljene na pravilima.</span><span class="sxs-lookup"><span data-stu-id="d600f-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="d600f-115">Q Ako je uređaj šifriran kao rezultat primjene pravila intune će se dešifrirati kada se to pravilo ukloni?</span><span class="sxs-lookup"><span data-stu-id="d600f-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="d600f-116">O: Uklanjanje pravila vezanih uz šifriranje NE rezultira dešifrirati pogone koji su konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="d600f-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="d600f-117">P: Zašto pravila usklađivanja s usklađenošću pokazuju da moj uređaj nema "Bitlocker omogućen", ali jest?</span><span class="sxs-lookup"><span data-stu-id="d600f-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="d600f-118">O: Postavka "Bitlocker omogućena" u pravilniku o usklađenosti u usklađivanju koristi klijent za provjeru stanja uređaja u sustavu Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="d600f-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="d600f-119">Ovaj klijent mjeri samo stanje uređaja u vrijeme pokretanja.</span><span class="sxs-lookup"><span data-stu-id="d600f-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="d600f-120">Dakle, ako uređaj nije ponovno podizanje sustava od bitlocker šifriranje je dovršen DHA klijent usluga neće prijaviti bitlocker kao aktivan.</span><span class="sxs-lookup"><span data-stu-id="d600f-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>