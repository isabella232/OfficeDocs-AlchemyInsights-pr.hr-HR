---
title: Otklanjanje poteškoća s prijavom uređaja sa sustavom Windows u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665824"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="67443-102">Otklanjanje poteškoća s prijavom uređaja sa sustavom Windows u Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="67443-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="67443-103">Pregledajte resurse navedene u nastavku da biste odmah riješili problem.</span><span class="sxs-lookup"><span data-stu-id="67443-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="67443-104">Neke uobičajene poruke o pogreškama i koraci razlučivosti:</span><span class="sxs-lookup"><span data-stu-id="67443-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="67443-105">**Softver se ne može instalirati, 0x80cf4017:** Certifikat računa je istekao.</span><span class="sxs-lookup"><span data-stu-id="67443-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="67443-106">Ponovno preuzmite softverski paket PC Klijent u Intune Admin Console.</span><span class="sxs-lookup"><span data-stu-id="67443-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="67443-107">Dodatne informacije potražite u ovoj dokumentaciji.</span><span class="sxs-lookup"><span data-stu-id="67443-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="67443-108">**Kod pogreške 0x801c0003:** Pogreška se može pojaviti u sljedećim scenarijima:</span><span class="sxs-lookup"><span data-stu-id="67443-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="67443-109">Korisnik ima više uređaja upisanih od ograničenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="67443-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="67443-110">Pregledajte te dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="67443-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="67443-111">"Korisnici se mogu pridružiti uređajima azure AD" postavljeno je na "ništa".</span><span class="sxs-lookup"><span data-stu-id="67443-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="67443-112">Postavite ga na sve ili odaberite korisnike.</span><span class="sxs-lookup"><span data-stu-id="67443-112">Set it to all or select users.</span></span> <span data-ttu-id="67443-113">Dodatne informacije potražite [u ovoj dokumentaciji.](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)</span><span class="sxs-lookup"><span data-stu-id="67443-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="67443-114">Uređaj je već upisao drugi korisnik.</span><span class="sxs-lookup"><span data-stu-id="67443-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="67443-115">Ako je to slučaj, uklonite uređaj s konzole Azure Intune ili ručno odete uređaj prije ponovnog pokušaja.</span><span class="sxs-lookup"><span data-stu-id="67443-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="67443-116">Uređaj je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="67443-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="67443-117">Samo SE JSK-ovi za Windows 10 Pro, Education i Enterprise mogu pridružiti servisu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="67443-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="67443-118">Dodatni resursi koji olakšavaju rješavanje problema:</span><span class="sxs-lookup"><span data-stu-id="67443-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="67443-119">[Koristite Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene pogreške u prijavi.</span><span class="sxs-lookup"><span data-stu-id="67443-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="67443-120">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="67443-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="67443-121">Pregledajte popis uobičajenih pogrešaka koje sprječavaju prijavu i rješenja u svaki: Vodič za [otklanjanje poteškoća](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i Dokument za [otklanjanje poteškoća](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="67443-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="67443-122">[Saznajte kako prijaviti uređaje sa sustavom Windows u Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="67443-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
