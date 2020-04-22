---
title: Otklanjanje poteškoća s prijavom Android uređaja u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759612"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="b6f6b-102">Otklanjanje poteškoća s prijavom Android uređaja u Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b6f6b-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="b6f6b-103">Pregledajte dolje navedene resurse da biste riješili problem.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="b6f6b-104">Neki uobičajeni problemi i koraci rješavanja:</span><span class="sxs-lookup"><span data-stu-id="b6f6b-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="b6f6b-105">**Uređaj nije šifrirana pogreška na portalu tvrtke:** Novije verzije Androida, osobito počevši od v7.0, zahtijevaju šifru za pokretanje kako bi se osiguralo da je vaš uređaj u potpunosti šifriran.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="b6f6b-106">Uobičajena su rješenja omogućiti pribadaču za pokretanje ili potpuno šifrirati uređaj.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="b6f6b-107">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) za više informacija.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="b6f6b-108">**Uređaji propust to check in sa Intune poslužitelj ili otkriti kao " nezdrav" in Intune admin utješiti:** Neki uređaji Samsung 4.4 i 5.5 možda se neće prijaviti na uslugu.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="b6f6b-109">Postoje 3 moguća rješenja za ovaj problem:</span><span class="sxs-lookup"><span data-stu-id="b6f6b-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="b6f6b-110">Ručno otvorite aplikaciju Intune Portal tvrtke koja će automatski pokrenuti sinkronizaciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="b6f6b-111">Ažurirajte uređaj na Android 6.0 ili noviji.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="b6f6b-112">Onemogućite Samsung Smart Manager u upravljanju portalom tvrtke Intune.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="b6f6b-113">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za dodatne pojedinosti o tim pitanjima i rješenjima.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="b6f6b-114">**Vrsta licence korisnika Nije valjano** ili **korisničko ime nije prepoznato:** korisniku treba dodijeliti Intune ili EMS licencu.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="b6f6b-115">Pregledajte te dokumente da biste dodijelili licencu putem: Office Admin Center ili Portal azure.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="b6f6b-116">Dodatni resursi koji će vam pomoći u rješavanju problema:</span><span class="sxs-lookup"><span data-stu-id="b6f6b-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b6f6b-117">Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene pogreške pri upisu.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b6f6b-118">Dodatne informacije potražite [u ovom dokumentu.](https://docs.microsoft.com/intune/help-desk-operators)</span><span class="sxs-lookup"><span data-stu-id="b6f6b-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="b6f6b-119">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za popis uobičajenih pogrešaka koje sprječavaju prijavu i rješenja za svaku od njih.</span><span class="sxs-lookup"><span data-stu-id="b6f6b-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="b6f6b-120">[Saznajte kako prijaviti Android uređaje u Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="b6f6b-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
