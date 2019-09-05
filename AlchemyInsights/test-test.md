---
title: Uvjeti nedostaju iz spremišta termina Online SharePoint
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762045"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="475f6-102">Omogućivanja Bitlocker šifriranja s Intune</span><span class="sxs-lookup"><span data-stu-id="475f6-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="475f6-103">Pravila zaštite Intune krajnje točke mogu se konfigurirati postavke šifriranja Boitlocker za uređaje sustava Windows kao što je opisano u: Windows10 (i novijima) postavke za zaštitu uređaja pomoću Intune</span><span class="sxs-lookup"><span data-stu-id="475f6-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="475f6-104">Imajte na umu da mnogi uređaji novija izvodi Windows 10 podržava automatsko bitlocker šifriranje koje je pokrenulo bez aplikacije MDM pravila.</span><span class="sxs-lookup"><span data-stu-id="475f6-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="475f6-105">Aplikacija pravila to utjecati ako konfigurirane postavke koje nisu zadane.</span><span class="sxs-lookup"><span data-stu-id="475f6-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="475f6-106">Više detalja potražite u odjeljku najčešća pitanja vezana uz.</span><span class="sxs-lookup"><span data-stu-id="475f6-106">See FAQ for more detail.</span></span>


<span data-ttu-id="475f6-107">Najčešća pitanja vezana uz  Q: koje izdanjima sustava Windows podržava uređaj šifriranje pomoću pravila zaštite krajnja točka?</span><span class="sxs-lookup"><span data-stu-id="475f6-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="475f6-108"> A: postavke u pravilima zaštite krajnje točke Intune su implementirati pomoću Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="475f6-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="475f6-109">Nisu sve izdanja niti izgradi Windows podržava Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="475f6-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="475f6-110">Na ovom vrijeme izdanja sustava Windows: Enterprise; Podržane su Obrazovanje, mobilni, mobilni Enterprise i Professional (iz build 1809 nadalje).</span><span class="sxs-lookup"><span data-stu-id="475f6-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="475f6-111">Q: Ako uređaj već šifriran pomoću Bitlocker koristeći zadane postavke OS za metodu šifriranja i snaga šifriranja (XTS-AES-128) će Primjena pravila s različitim postavkama automatski okidač ponovnog šifriranja pogona s nove postavke?</span><span class="sxs-lookup"><span data-stu-id="475f6-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="475f6-112">A: Br.</span><span class="sxs-lookup"><span data-stu-id="475f6-112">A: No.</span></span> <span data-ttu-id="475f6-113">Za primjenu nove postavke snaga moraju prvo dešifrirati pogon.</span><span class="sxs-lookup"><span data-stu-id="475f6-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="475f6-114">Napomena za uređaje koji se upisani s Autopilot automatsko šifriranje koje bi doći tijekom OOBE se aktivira dok Intune pravila vrednovanja koja omogućuje pravila temelji postavke koristiti umjesto zadanih postavki OS</span><span class="sxs-lookup"><span data-stu-id="475f6-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="475f6-115">Q ako uređaj šifrirani zbog aplikacije pravila Intune će ga se dešifrirati kada se uklone tog pravila?</span><span class="sxs-lookup"><span data-stu-id="475f6-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="475f6-116">A: uklanjanje šifriranja Srodni pravila rezultirati dešifriranje pogona koji su konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="475f6-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="475f6-117">Q: Zašto se intune pravila usklađenosti ne Pokaži moj uređaj imaju "Omogućeno Bitlocker", ali je?</span><span class="sxs-lookup"><span data-stu-id="475f6-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="475f6-118">A: na "Bitlocker omogućeno" postavka pravila usklađenosti intune koristi klijent Windows uređaj stanja Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="475f6-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="475f6-119">Ovaj klijent samo mjeri stanje uređaja prilikom pokretanja.</span><span class="sxs-lookup"><span data-stu-id="475f6-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="475f6-120">Tako ako uređaj ne sustava nakon dovršetka bitlocker šifriranje klijentski servis DHA će izvješće bitlocker kao aktivni.</span><span class="sxs-lookup"><span data-stu-id="475f6-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>