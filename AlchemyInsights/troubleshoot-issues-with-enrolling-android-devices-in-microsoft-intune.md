---
title: Otklanjanje poteškoća s upisivanjem uređaja sa sustavom Android u programu Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708990"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="280b8-102">Otklanjanje poteškoća s upisivanjem uređaja sa sustavom Android u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="280b8-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="280b8-103">Pregledajte navedene resurse da biste sada riješili problem.</span><span class="sxs-lookup"><span data-stu-id="280b8-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="280b8-104">Neki Česti problemi i koraci sanacije:</span><span class="sxs-lookup"><span data-stu-id="280b8-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="280b8-105">**Pogreška uređaja nije šifrirana na portalu tvrtke:** Novije verzije sustava Android, posebno Počevši od v 7.0, zahtijevaju lozinku za pokretanje da biste provjerili je li vaš uređaj potpuno šifriran.</span><span class="sxs-lookup"><span data-stu-id="280b8-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="280b8-106">Najčešća rješenja jesu omogućivanje PIN-a za pokretanje ili potpuno šifriranje uređaja.</span><span class="sxs-lookup"><span data-stu-id="280b8-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="280b8-107">Dodatne informacije potražite u [ovom dokumentu](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .</span><span class="sxs-lookup"><span data-stu-id="280b8-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="280b8-108">**Uređaji se ne mogu prijaviti pomoću servisa Intune ili prikaza kao "nezdravih" u konzoli za administratore:** Neki uređaji za Samsung 4,4 i 5,5 možda se neće prijaviti u servis.</span><span class="sxs-lookup"><span data-stu-id="280b8-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="280b8-109">U ovom problemu postoje tri moguća rješenja:</span><span class="sxs-lookup"><span data-stu-id="280b8-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="280b8-110">Ručno otvorite aplikaciju Intune Company portal koja će automatski pokrenuti sinkronizaciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="280b8-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="280b8-111">Ažurirajte uređaj na Android 6,0 ili noviji.</span><span class="sxs-lookup"><span data-stu-id="280b8-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="280b8-112">Onemogućite Samsung Smart Manager da upravlja putem portala Intune Company.</span><span class="sxs-lookup"><span data-stu-id="280b8-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="280b8-113">Pregledajte [ovaj dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) da biste saznali više o tim pitanjima i rezolucijama.</span><span class="sxs-lookup"><span data-stu-id="280b8-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="280b8-114">**Vrsta korisničke licence nije valjana** ili **korisničko ime nije prepoznata pogreška:** korisniku je potrebno dodijeliti licencu za Intune ili EMS.</span><span class="sxs-lookup"><span data-stu-id="280b8-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="280b8-115">Pregledajte ove dokumente da biste dodijelili licencu putem: centar za administratore sustava Office ili portal Azure.</span><span class="sxs-lookup"><span data-stu-id="280b8-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="280b8-116">Dodatni resursi koji će vam olakšati rješavanje problema:</span><span class="sxs-lookup"><span data-stu-id="280b8-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="280b8-117">Koristite [portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili česte neuspjehe upisa.</span><span class="sxs-lookup"><span data-stu-id="280b8-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="280b8-118">Dodatne pojedinosti potražite u [ovom dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="280b8-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="280b8-119">Pregledajte [ovaj dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) radi popisa uobičajenih pogrešaka koji sprječavaju upis i rezolucije na svaki od njih.</span><span class="sxs-lookup"><span data-stu-id="280b8-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="280b8-120">Upute [za upis uređaja sa sustavom Android u programu Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="280b8-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
