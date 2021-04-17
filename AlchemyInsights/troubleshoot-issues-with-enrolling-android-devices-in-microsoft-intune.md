---
title: Otklanjanje poteškoća s registracijom uređaja sa sustavom Android u aplikaciji Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830934"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="59e81-102">Otklanjanje poteškoća s registracijom uređaja sa sustavom Android u aplikaciji Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="59e81-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="59e81-103">Pregledajte resurse navedene u nastavku da biste odmah riješili problem.</span><span class="sxs-lookup"><span data-stu-id="59e81-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="59e81-104">Neki uobičajeni problemi i koraci za rješavanje:</span><span class="sxs-lookup"><span data-stu-id="59e81-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="59e81-105">**Pogreška uređaja nije šifrirana na portalu tvrtke:** Novije verzije sustava Android, osobito počevši od verzije v7.0, zahtijevaju pristupnu šifru za pokretanje da biste bili sigurni da je uređaj u potpunosti šifriran.</span><span class="sxs-lookup"><span data-stu-id="59e81-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="59e81-106">Uobičajena su rješenja omogućivanje pribadače za pokretanje ili potpuno šifriranje uređaja.</span><span class="sxs-lookup"><span data-stu-id="59e81-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="59e81-107">Dodatne [informacije potražite](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) u ovom dokumentu.</span><span class="sxs-lookup"><span data-stu-id="59e81-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="59e81-108">**Uređaji se ne prijave pomoću servisa Intune ili se prikazuju kao "nezdravi" na administratorskim konzolama aplikacije Intune:** Neki uređaji Samsung 4.4 i 5.5 možda se ne prijave u servis.</span><span class="sxs-lookup"><span data-stu-id="59e81-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="59e81-109">Za taj problem postoje tri moguća rješenja:</span><span class="sxs-lookup"><span data-stu-id="59e81-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="59e81-110">Ručno otvorite aplikaciju Intune Company Portal, koja će automatski pokrenuti sinkronizaciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="59e81-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="59e81-111">Ažurirajte uređaj na Android 6.0 ili noviji.</span><span class="sxs-lookup"><span data-stu-id="59e81-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="59e81-112">Onemogućite Samsung Smart Manager da upravlja portalom Tvrtke Intune.</span><span class="sxs-lookup"><span data-stu-id="59e81-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="59e81-113">Pregledajte [ovaj dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) da biste vidjeli dodatne pojedinosti o tim problemima i rješavanjima.</span><span class="sxs-lookup"><span data-stu-id="59e81-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="59e81-114">**Pogreška Vrsta korisničke licence nije** **valjana ili** korisničko ime nije prepoznato: korisniku je potrebno dodijeliti licencu za Intune ili EMS.</span><span class="sxs-lookup"><span data-stu-id="59e81-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="59e81-115">Pregledajte ove dokumente da biste dodijelili licencu putem: Centra za administratore sustava Office ili portala Azure.</span><span class="sxs-lookup"><span data-stu-id="59e81-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="59e81-116">Dodatni resursi za rješavanje problema:</span><span class="sxs-lookup"><span data-stu-id="59e81-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="59e81-117">Pomoću [portala za otklanjanje poteškoća sa servisom Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) dijagnosticirajte i riješite uobičajene pogreške prilikom prijave.</span><span class="sxs-lookup"><span data-stu-id="59e81-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="59e81-118">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) da biste saznali više.</span><span class="sxs-lookup"><span data-stu-id="59e81-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="59e81-119">Pregledajte [ovaj dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) da biste pregledali popis uobičajenih pogrešaka koje sprječavaju registraciju i rješenja za svaku od njih.</span><span class="sxs-lookup"><span data-stu-id="59e81-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="59e81-120">[Saznajte kako prijaviti uređaje sa sustavom Android u Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="59e81-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
