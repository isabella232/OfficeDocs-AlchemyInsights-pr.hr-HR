---
title: Otklanjanje poteškoća s registracijom uređaja sa sustavom Windows u aplikaciji Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808963"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="d5550-102">Otklanjanje poteškoća s registracijom uređaja sa sustavom Windows u aplikaciji Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d5550-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="d5550-103">Pregledajte resurse navedene u nastavku da biste odmah riješili problem.</span><span class="sxs-lookup"><span data-stu-id="d5550-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d5550-104">Neke uobičajene poruke o pogreškama i koraci za rješavanje:</span><span class="sxs-lookup"><span data-stu-id="d5550-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="d5550-105">**Softver nije moguće instalirati, 0x80cf4017:** Vaš je certifikat računa istekao.</span><span class="sxs-lookup"><span data-stu-id="d5550-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="d5550-106">Ponovno preuzmite softverski paket klijentskog računala na konzoli za administratore aplikacije Intune.</span><span class="sxs-lookup"><span data-stu-id="d5550-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="d5550-107">Dodatne informacije potražite u ovoj dokumentaciji.</span><span class="sxs-lookup"><span data-stu-id="d5550-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="d5550-108">**Kod pogreške 0x801c0003:** Pogreška se može pojaviti u sljedećim scenarijima:</span><span class="sxs-lookup"><span data-stu-id="d5550-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="d5550-109">Korisnik ima više uređaja koji su upisani od ograničenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="d5550-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="d5550-110">Pregledajte te [dokumente da biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) [ili promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="d5550-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="d5550-111">"Korisnici se mogu pridružiti uređajima na servisu Azure AD" postavljen je na "none".</span><span class="sxs-lookup"><span data-stu-id="d5550-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="d5550-112">Postavite je na sve ili odaberite korisnike.</span><span class="sxs-lookup"><span data-stu-id="d5550-112">Set it to all or select users.</span></span> <span data-ttu-id="d5550-113">Dodatne [informacije potražite](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) u ovoj dokumentaciji.</span><span class="sxs-lookup"><span data-stu-id="d5550-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="d5550-114">Uređaj je već prijavio drugi korisnik.</span><span class="sxs-lookup"><span data-stu-id="d5550-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="d5550-115">U tom slučaju uklonite uređaj s konzole Azure Intune ili ručno poništite zahtjev uređaja prije nego što ga ponovno počnete pokušavati.</span><span class="sxs-lookup"><span data-stu-id="d5550-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="d5550-116">Uređaj je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="d5550-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="d5550-117">Samo SKU-i za Windows 10 Pro, Education i Enterprise mogu se pridružiti servisu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d5550-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="d5550-118">Dodatni resursi za rješavanje problema:</span><span class="sxs-lookup"><span data-stu-id="d5550-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="d5550-119">Pomoću [portala za otklanjanje poteškoća sa servisom Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) dijagnosticirajte i riješite uobičajene pogreške prilikom prijave.</span><span class="sxs-lookup"><span data-stu-id="d5550-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d5550-120">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) da biste saznali više.</span><span class="sxs-lookup"><span data-stu-id="d5550-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="d5550-121">Pregledajte ove dokumente da biste pregledali popis uobičajenih pogrešaka koje sprječavaju prijavu i rješenja za svaku od njih: vodič za otklanjanje [poteškoća i dokument](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) za otklanjanje [poteškoća.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="d5550-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="d5550-122">[Saznajte kako registrirati uređaje sa sustavom Windows u aplikaciji Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="d5550-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
