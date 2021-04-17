---
title: Otklanjanje poteškoća s registracijom uređaja sa sustavom iOS u aplikaciji Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823455"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="d76a1-102">Otklanjanje poteškoća s registracijom uređaja sa sustavom iOS u aplikaciji Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d76a1-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="d76a1-103">Pregledajte resurse navedene u nastavku da biste odmah riješili problem.</span><span class="sxs-lookup"><span data-stu-id="d76a1-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="d76a1-104">Neke uobičajene poruke o pogreškama i koraci za rješavanje:</span><span class="sxs-lookup"><span data-stu-id="d76a1-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="d76a1-105">**Dosegnut je cap device cap** Korisnik ima više uređaja koji su upisani od ograničenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="d76a1-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="d76a1-106">Pregledajte te [dokumente da biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) [ili promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="d76a1-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="d76a1-107">**Ovaj servis nije podržan. Bez pravilnika za prijavu:** Appleov servis za automatsko obavještavanje (APNS) mora se konfigurirati ili obnoviti.</span><span class="sxs-lookup"><span data-stu-id="d76a1-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="d76a1-108">Upute [za to](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) potražite u ovom dokumentu.</span><span class="sxs-lookup"><span data-stu-id="d76a1-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="d76a1-109">**Vrsta korisničke licence nije valjana ili korisničko ime nije prepoznato:** Korisniku je potrebno dodijeliti licencu za Intune ili EMS.</span><span class="sxs-lookup"><span data-stu-id="d76a1-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d76a1-110">Pregledajte ove dokumente da biste dodijelili licencu putem: [Centra za administratore sustava Office](https://docs.microsoft.com/intune/licenses-assign) ili [portala Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="d76a1-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="d76a1-111">Dodatni resursi za rješavanje problema:</span><span class="sxs-lookup"><span data-stu-id="d76a1-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d76a1-112">Pomoću [portala za otklanjanje poteškoća sa servisom Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) dijagnosticirajte i riješite uobičajene pogreške prilikom prijave.</span><span class="sxs-lookup"><span data-stu-id="d76a1-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d76a1-113">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) da biste saznali više.</span><span class="sxs-lookup"><span data-stu-id="d76a1-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="d76a1-114">Pregledajte ove dokumente da biste pregledali popis uobičajenih pogrešaka koje sprječavaju prijavu i rješenja za svaku od njih: vodič za otklanjanje [poteškoća i dokument](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) za otklanjanje [poteškoća.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="d76a1-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="d76a1-115">[Saznajte kako registrirati uređaje sa sustavom iOS u aplikaciji Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="d76a1-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

