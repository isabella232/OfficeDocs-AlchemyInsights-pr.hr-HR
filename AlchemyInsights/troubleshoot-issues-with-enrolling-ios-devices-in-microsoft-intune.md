---
title: Otklanjanje poteškoća s upisom iOS uređaja u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506913"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="8e348-102">Otklanjanje poteškoća s upisom iOS uređaja u Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="8e348-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="8e348-103">Pregledajte dolje navedene resurse da biste sada riješili problem.</span><span class="sxs-lookup"><span data-stu-id="8e348-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="8e348-104">Neke uobičajene poruke o pogrešci i koraci rezolucije:</span><span class="sxs-lookup"><span data-stu-id="8e348-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="8e348-105">**Dosegnut zatvarač uređaja** Korisnik ima više uređaja uključenih od ograničenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="8e348-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="8e348-106">Pregledajte ove dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="8e348-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="8e348-107">**Ova usluga nije podržana. Nema pravila o prijavi:** Apple push, usluga obavješćivanja (APNS) treba konfigurirati ili obnoviti.</span><span class="sxs-lookup"><span data-stu-id="8e348-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="8e348-108">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) za upute o tome kako to učiniti.</span><span class="sxs-lookup"><span data-stu-id="8e348-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="8e348-109">**Vrsta licence za korisnika nije valjana ili korisničko ime nije prepoznano:** Korisniku treba dodijeliti licencu Intune ili EMS.</span><span class="sxs-lookup"><span data-stu-id="8e348-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="8e348-110">Pregledajte ove dokumente da biste dodijelili licencu putem: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) ili [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="8e348-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="8e348-111">Dodatni resursi koji pomažu u rješavanju problema:</span><span class="sxs-lookup"><span data-stu-id="8e348-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="8e348-112">Koristite [Intune otklanjanje poteškoća portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) za dijagnosticiranje i rješavanje uobičajenih neuspjeha prijave.</span><span class="sxs-lookup"><span data-stu-id="8e348-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="8e348-113">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="8e348-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="8e348-114">Pregledajte ove dokumente za popis uobičajenih pogrešaka koje sprječavaju upis i rezoluciju za svaki: [Vodič za otklanjanje poteškoća](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i pri [rješavanju problema](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="8e348-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="8e348-115">[Saznajte kako upisati iOS uređaje u Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="8e348-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

