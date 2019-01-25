---
title: Rješavanje problema s uvrštavate Windows uređaja u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29461845"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="44676-102">Rješavanje problema s uvrštavate Windows uređaja u Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="44676-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="44676-103">Pregledajte resurse dolje navedene da riješite problem.</span><span class="sxs-lookup"><span data-stu-id="44676-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="44676-104">Neke uobičajene poruke o pogreškama i razlučivost korake:</span><span class="sxs-lookup"><span data-stu-id="44676-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="44676-p101">**Ne može biti instaliran softver, 0x80cf4017:** Račun certifikat je istekao. Ponovno preuzmite paket PC klijentski softver u Intune administratorske konzole. Pregledajte dokumentaciju za dodatne informacije.</span><span class="sxs-lookup"><span data-stu-id="44676-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="44676-108">**0x801c0003 Šifra pogreške:** Pogreška se može pojaviti u sljedećim scenarijima:</span><span class="sxs-lookup"><span data-stu-id="44676-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="44676-p102">Korisnik ima više uređaja upisani od ograničenja uređaja. Pregledajte te dokumente [ukloniti uređaj](https://docs.microsoft.com/en-us/intune/devices-wipe) ili [promijeniti ograničenje uređaja](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="44676-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="44676-p103">"Korisnici možda pridružite uređaji Azure AD" postavite na "none". Postavljanje svim ili odaberite korisnika. Pregledajte [ove dokumentacije](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) za dodatne informacije.</span><span class="sxs-lookup"><span data-stu-id="44676-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="44676-p104">Uređaj već upisani drugi korisnik. Ako je to slučaj, uklonite uređaj iz konzole Azure Intune ili ručno unenroll uređaja prije ponovnog pokušaja.</span><span class="sxs-lookup"><span data-stu-id="44676-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="44676-p105">Uređaj je Windows 10 Home. Samo Windows 10 Pro, obrazovanje i Enterprise JSK možete pridružiti Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="44676-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="44676-118">Dodatne resurse za pomoć riješiti vaš problem:</span><span class="sxs-lookup"><span data-stu-id="44676-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="44676-p106">Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene neuspjeha uvrštenje. Pregledajte [ovaj dokument](https://docs.microsoft.com/en-us/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="44676-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="44676-121">Pregledajte te dokumente za popis uobičajene pogreške koje sprječavaju uvrštenje i rješenja za svaki: [Vodič za otklanjanje poteškoća](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Otklanjanje poteškoća doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="44676-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="44676-122">[Saznajte kako da biste uvrstili Windows uređaja u Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="44676-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

