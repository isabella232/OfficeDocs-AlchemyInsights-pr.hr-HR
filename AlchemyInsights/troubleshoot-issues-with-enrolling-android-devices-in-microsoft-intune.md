---
title: Rješavanje problema s uvrštavate Android uređaja Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500063"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="a7268-102">Rješavanje problema s uvrštavate Android uređaja Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a7268-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="a7268-103">Pregledajte resurse dolje navedene da riješite problem.</span><span class="sxs-lookup"><span data-stu-id="a7268-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="a7268-104">Neke uobičajene probleme i rješenja korake:</span><span class="sxs-lookup"><span data-stu-id="a7268-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="a7268-105">**Uređaj nije šifrirana pogreška u poduzeću Portal:** Novije verzije Android, osobito počevši s v7.0, zahtijevaju pokretanje "passcode" da biste bili sigurni da uređaj u potpunosti šifrirana.</span><span class="sxs-lookup"><span data-stu-id="a7268-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="a7268-106">Da biste omogućili pin za pokretanje ili potpuno šifriranje uređaj su uobičajene rješenja.</span><span class="sxs-lookup"><span data-stu-id="a7268-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="a7268-107">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) dodatne informacije.</span><span class="sxs-lookup"><span data-stu-id="a7268-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="a7268-108">**Uređaji neće uspjeti za provjeru pomoću servisa Intune ili prikazati kao "Unhealthy" u administratorske konzole Intune:** Neke 4.4 Samsung i 5.5 uređaji možda provjerite u servis.</span><span class="sxs-lookup"><span data-stu-id="a7268-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="a7268-109">Postoje 3 mogućih rješenja za ovaj problem:</span><span class="sxs-lookup"><span data-stu-id="a7268-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="a7268-110">Ručno otvaranje app Portal tvrtke Intune koji će automatski započeti sinkronizaciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="a7268-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="a7268-111">Ažuriranje uređaja na Android 6.0 ili noviji.</span><span class="sxs-lookup"><span data-stu-id="a7268-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="a7268-112">Onemogući upravitelja pametne Samsung iz upravljanje Portal tvrtke Intune.</span><span class="sxs-lookup"><span data-stu-id="a7268-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="a7268-113">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za daljnje pojedinosti o ti problemi i rješenja.</span><span class="sxs-lookup"><span data-stu-id="a7268-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="a7268-114">**Korisničke licence vrsta valjan** ili **korisničko ime nije prepoznato pogreška:** korisnik mora biti dodijeljen Intune ili EMS licence.</span><span class="sxs-lookup"><span data-stu-id="a7268-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="a7268-115">Pregledajte te dokumente dodeljivanje licence kroz: Office Admin centar ili Azure portal.</span><span class="sxs-lookup"><span data-stu-id="a7268-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="a7268-116">Dodatne resurse za pomoć riješiti vaš problem:</span><span class="sxs-lookup"><span data-stu-id="a7268-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="a7268-117">Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene neuspjeha uvrštenje.</span><span class="sxs-lookup"><span data-stu-id="a7268-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a7268-118">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="a7268-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="a7268-119">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za popis uobičajene pogreške koje sprječavaju uvrštenje i rješenja za svaki.</span><span class="sxs-lookup"><span data-stu-id="a7268-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="a7268-120">[Saznajte kako da biste uvrstili Android uređaja Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="a7268-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
