---
title: Otklanjanje poteškoća s prijavom iOS uređaja u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736150"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="4e523-102">Otklanjanje poteškoća s prijavom iOS uređaja u Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4e523-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="4e523-103">Pregledajte dolje navedene resurse da biste riješili problem.</span><span class="sxs-lookup"><span data-stu-id="4e523-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="4e523-104">Neke uobičajene poruke o pogreškama i koraci rješenja:</span><span class="sxs-lookup"><span data-stu-id="4e523-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="4e523-105">**Dosegnuta je gornja granica uređaja** Korisnik ima više uređaja prijavljenih od ograničenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="4e523-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="4e523-106">Pregledajte te dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="4e523-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="4e523-107">**Ova usluga nije podržana. Nema pravila za prijavu:** Appleovu uslugu obavještavanja o pushu (APNS) potrebno je konfigurirati ili obnoviti.</span><span class="sxs-lookup"><span data-stu-id="4e523-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="4e523-108">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) za upute o tome kako to učiniti.</span><span class="sxs-lookup"><span data-stu-id="4e523-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="4e523-109">**Vrsta licence korisnika nije valjana ili korisničko ime nije prepoznato:** Korisniku treba dodijeliti Intune ili EMS licencu.</span><span class="sxs-lookup"><span data-stu-id="4e523-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="4e523-110">Pregledajte te dokumente da biste dodijelili licencu putem: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) ili Portal [azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="4e523-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="4e523-111">Dodatni resursi koji će vam pomoći u rješavanju problema:</span><span class="sxs-lookup"><span data-stu-id="4e523-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="4e523-112">Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene pogreške pri upisu.</span><span class="sxs-lookup"><span data-stu-id="4e523-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="4e523-113">Dodatne informacije potražite [u ovom dokumentu.](https://docs.microsoft.com/intune/help-desk-operators)</span><span class="sxs-lookup"><span data-stu-id="4e523-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="4e523-114">Pregledajte te dokumente za popis uobičajenih pogrešaka koje sprječavaju prijavu i rješenja za svaku: [Vodič za otklanjanje poteškoća](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i Otklanjanje poteškoća [.](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="4e523-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="4e523-115">[Saznajte kako prijaviti iOS uređaje u microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="4e523-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

