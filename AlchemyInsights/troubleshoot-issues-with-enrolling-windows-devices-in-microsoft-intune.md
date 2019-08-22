---
title: Rješavanje problema s uvrštavate Windows uređaja u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559653"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="3511d-102">Rješavanje problema s uvrštavate Windows uređaja u Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3511d-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="3511d-103">Pregledajte resurse dolje navedene da riješite problem.</span><span class="sxs-lookup"><span data-stu-id="3511d-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="3511d-104">Neke uobičajene poruke o pogreškama i razlučivost korake:</span><span class="sxs-lookup"><span data-stu-id="3511d-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="3511d-105">**Ne može biti instaliran softver, 0x80cf4017:** Račun certifikat je istekao.</span><span class="sxs-lookup"><span data-stu-id="3511d-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="3511d-106">Ponovno preuzmite paket PC klijentski softver u Intune administratorske konzole.</span><span class="sxs-lookup"><span data-stu-id="3511d-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="3511d-107">Pregledajte dokumentaciju za dodatne informacije.</span><span class="sxs-lookup"><span data-stu-id="3511d-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="3511d-108">**0x801c0003 Šifra pogreške:** Pogreška se može pojaviti u sljedećim scenarijima:</span><span class="sxs-lookup"><span data-stu-id="3511d-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="3511d-109">Korisnik ima više uređaja upisani od ograničenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="3511d-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="3511d-110">Pregledajte te dokumente [ukloniti uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promijeniti ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="3511d-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="3511d-111">"Korisnici možda pridružite uređaji Azure AD" postavite na "none".</span><span class="sxs-lookup"><span data-stu-id="3511d-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="3511d-112">Postavljanje svim ili odaberite korisnika.</span><span class="sxs-lookup"><span data-stu-id="3511d-112">Set it to all or select users.</span></span> <span data-ttu-id="3511d-113">Pregledajte [ove dokumentacije](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za dodatne informacije.</span><span class="sxs-lookup"><span data-stu-id="3511d-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="3511d-114">Uređaj već upisani drugi korisnik.</span><span class="sxs-lookup"><span data-stu-id="3511d-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="3511d-115">Ako je to slučaj, uklonite uređaj iz konzole Azure Intune ili ručno unenroll uređaja prije ponovnog pokušaja.</span><span class="sxs-lookup"><span data-stu-id="3511d-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="3511d-116">Uređaj je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="3511d-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="3511d-117">Samo Windows 10 Pro, obrazovanje i Enterprise JSK možete pridružiti Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3511d-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="3511d-118">Dodatne resurse za pomoć riješiti vaš problem:</span><span class="sxs-lookup"><span data-stu-id="3511d-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="3511d-119">Koristite [Intune Portal za otklanjanje poteškoća](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnosticirali i riješili uobičajene neuspjeha uvrštenje.</span><span class="sxs-lookup"><span data-stu-id="3511d-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3511d-120">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="3511d-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="3511d-121">Pregledajte te dokumente za popis uobičajene pogreške koje sprječavaju uvrštenje i rješenja za svaki: [Vodič za otklanjanje poteškoća](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Otklanjanje poteškoća doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="3511d-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="3511d-122">[Saznajte kako da biste uvrstili Windows uređaja u Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="3511d-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
