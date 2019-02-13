---
title: Rješavanje problema s uvrštavate iOS uređaja u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924760"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="ab2ab-102">Rješavanje problema s uvrštavate iOS uređaja u Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ab2ab-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="ab2ab-103">Pregledajte resurse dolje navedene da riješite problem.</span><span class="sxs-lookup"><span data-stu-id="ab2ab-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="ab2ab-104">Neke uobičajene poruke o pogreškama i razlučivost korake:</span><span class="sxs-lookup"><span data-stu-id="ab2ab-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="ab2ab-p101">**Dostignuto pokrova uređaja** Korisnik ima više uređaja upisani od ograničenja uređaja. Pregledajte te dokumente [ukloniti uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijeniti ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="ab2ab-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="ab2ab-p102">Ovaj servis **nije podržana. Nema pravila uvrštenje:** Apple Gurni obavijesti servisa (APN-ove) mora biti konfiguriran ili obnoviti. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) za upute kako to učiniti.</span><span class="sxs-lookup"><span data-stu-id="ab2ab-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="ab2ab-p103">**Nije valjana vrsta licence korisnika ili korisničko ime nije prepoznata:** Korisnik mora biti dodijeljen Intune ili EMS licence. Pregledajte te dokumente dodeljivanje licence kroz: [Office Admin centar](https://docs.microsoft.com/intune/licenses-assign) ili [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="ab2ab-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="ab2ab-111">Dodatne resurse za pomoć riješiti vaš problem:</span><span class="sxs-lookup"><span data-stu-id="ab2ab-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ab2ab-p104">Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene neuspjeha uvrštenje. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="ab2ab-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="ab2ab-114">Pregledajte te dokumente za popis uobičajene pogreške koje sprječavaju uvrštenje i rješenja za svaki: [Vodič za otklanjanje poteškoća](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [Otklanjanje poteškoća doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="ab2ab-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="ab2ab-115">[Saznajte kako da biste uvrstili iOS uređaja u Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="ab2ab-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

