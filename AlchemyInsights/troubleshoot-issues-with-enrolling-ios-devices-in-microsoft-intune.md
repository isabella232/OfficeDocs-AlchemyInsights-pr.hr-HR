---
title: Otklanjanje poteškoća s upisivanjem uređaja sa sustavom iOS u programu Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708954"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="e7c21-102">Otklanjanje poteškoća s upisivanjem uređaja sa sustavom iOS u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e7c21-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="e7c21-103">Pregledajte navedene resurse da biste sada riješili problem.</span><span class="sxs-lookup"><span data-stu-id="e7c21-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="e7c21-104">Neke česte poruke o pogreškama i koraci za rješavanje:</span><span class="sxs-lookup"><span data-stu-id="e7c21-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="e7c21-105">**Stigao je poklopac uređaja** Korisnik ima više uključenih uređaja od ograničenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="e7c21-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e7c21-106">Pregledajte ove dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="e7c21-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="e7c21-107">**Ovaj servis nije podržan. Nema pravilnika o upisu:** servis Apple push notifikacije (APN-ovi) mora biti konfiguriran ili obnovljen.</span><span class="sxs-lookup"><span data-stu-id="e7c21-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="e7c21-108">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) radi uputa o tome kako to učiniti.</span><span class="sxs-lookup"><span data-stu-id="e7c21-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="e7c21-109">**Vrsta korisničke licence nije valjana ili korisničko ime nije prepoznalo:** Korisniku je potrebno dodijeliti licencu za Intune ili EMS.</span><span class="sxs-lookup"><span data-stu-id="e7c21-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e7c21-110">Pregledajte ove dokumente da biste dodijelili licencu putem: [centar za administratore sustava Office](https://docs.microsoft.com/intune/licenses-assign) ili [portal Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="e7c21-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="e7c21-111">Dodatni resursi koji će vam olakšati rješavanje problema:</span><span class="sxs-lookup"><span data-stu-id="e7c21-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e7c21-112">Koristite [portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili česte neuspjehe upisa.</span><span class="sxs-lookup"><span data-stu-id="e7c21-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e7c21-113">Dodatne pojedinosti potražite u [ovom dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="e7c21-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="e7c21-114">Pregledajte ove dokumente za popis uobičajenih pogrešaka koje sprječavaju upis i rezolucije na svaki: upute za [Otklanjanje poteškoća](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [Otklanjanje poteškoća s liječnikom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e7c21-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="e7c21-115">Upute [za upis uređaja sa sustavom iOS u programu Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="e7c21-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

