---
title: Otklanjanje poteškoća s upisivanjem uređaja sa sustavom Windows u programu Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708882"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="11845-102">Otklanjanje poteškoća s upisivanjem uređaja sa sustavom Windows u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="11845-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="11845-103">Pregledajte navedene resurse da biste sada riješili problem.</span><span class="sxs-lookup"><span data-stu-id="11845-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="11845-104">Neke česte poruke o pogreškama i koraci za rješavanje:</span><span class="sxs-lookup"><span data-stu-id="11845-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="11845-105">**Softver se ne može instalirati, 0x80cf4017:** Potvrda računa je istekla.</span><span class="sxs-lookup"><span data-stu-id="11845-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="11845-106">Ponovno preuzmite računalni programski paket PC-ja u konzoli za administratore.</span><span class="sxs-lookup"><span data-stu-id="11845-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="11845-107">Dodatne informacije potražite u dokumentaciji.</span><span class="sxs-lookup"><span data-stu-id="11845-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="11845-108">**Kod pogreške 0x801c0003:** Pogreška se može pojaviti u sljedećim scenarijima:</span><span class="sxs-lookup"><span data-stu-id="11845-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="11845-109">Korisnik ima više uključenih uređaja od ograničenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="11845-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="11845-110">Pregledajte ove dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="11845-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="11845-111">"Korisnici se mogu pridružiti uređajima za Azure AD" postavljen je na "none".</span><span class="sxs-lookup"><span data-stu-id="11845-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="11845-112">Postavite ga na sve ili odaberite korisnike.</span><span class="sxs-lookup"><span data-stu-id="11845-112">Set it to all or select users.</span></span> <span data-ttu-id="11845-113">Dodatne informacije potražite u [dokumentaciji](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="11845-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="11845-114">Uređaj je već upisao neki drugi korisnik.</span><span class="sxs-lookup"><span data-stu-id="11845-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="11845-115">Ako je to slučaj, uklonite uređaj iz konzole Azure Intune ili ručno isključite uređaj prije ponovnog pokušaja.</span><span class="sxs-lookup"><span data-stu-id="11845-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="11845-116">Uređaj je Windows 10 home.</span><span class="sxs-lookup"><span data-stu-id="11845-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="11845-117">Samo Windows 10 Pro, Education i Enterprise SKUs mogu se pridružiti Azure Active direktoriju.</span><span class="sxs-lookup"><span data-stu-id="11845-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="11845-118">Dodatni resursi koji će vam olakšati rješavanje problema:</span><span class="sxs-lookup"><span data-stu-id="11845-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="11845-119">Koristite [portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili česte neuspjehe upisa.</span><span class="sxs-lookup"><span data-stu-id="11845-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="11845-120">Dodatne pojedinosti potražite u [ovom dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="11845-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="11845-121">Pregledajte ove dokumente za popis uobičajenih pogrešaka koje sprječavaju upis i rezolucije na svaki: upute za [Otklanjanje poteškoća](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Otklanjanje poteškoća s liječnikom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="11845-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="11845-122">[Naučite kako upisati uređaje sa sustavom Windows u programu Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="11845-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
