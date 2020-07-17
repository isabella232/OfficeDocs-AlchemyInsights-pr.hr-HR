---
title: Uvjetni pristup s intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931422"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="da4b3-102">Uvjetni pristup s intune</span><span class="sxs-lookup"><span data-stu-id="da4b3-102">Conditional Access with Intune</span></span>

<span data-ttu-id="da4b3-103">Korištenje **uvjetnog pristupa** s intune zahtijeva 3 koraka:</span><span class="sxs-lookup"><span data-stu-id="da4b3-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="da4b3-104">Stvorite **pravila usklađenosti** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) da biste definirali postavke koje se moraju ispuniti prije nego što se uređaj smatra sukladnim.</span><span class="sxs-lookup"><span data-stu-id="da4b3-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="da4b3-105">Na primjer, uređaj mora imati pribadaču od najmanje 6 znamenki prije nego što se smatra sukladnim.</span><span class="sxs-lookup"><span data-stu-id="da4b3-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="da4b3-106">Stvorite **pravilo uvjetnog pristupa** koje definira koji su resursi zaštićeni i koji uvjeti moraju biti ispunjeni za pristup tim resursima.</span><span class="sxs-lookup"><span data-stu-id="da4b3-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="da4b3-107">[Na primjer,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) uređaj mora biti sukladan prije pristupanja korporativnoj e-pošti.</span><span class="sxs-lookup"><span data-stu-id="da4b3-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="da4b3-108">Provjerite jesu li **pravila usklađenosti** i **pravila uvjetnog pristupa** usmjerena na željene grupe korisnika.</span><span class="sxs-lookup"><span data-stu-id="da4b3-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="da4b3-109">To može zahtijevati stvaranje određenih grupa korisnika u servisu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="da4b3-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="da4b3-110">**Korisni linkovi:**</span><span class="sxs-lookup"><span data-stu-id="da4b3-110">**Helpful links:**</span></span>

[<span data-ttu-id="da4b3-111">Pregled usklađenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="da4b3-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="da4b3-112">Rješavanje problema CA</span><span class="sxs-lookup"><span data-stu-id="da4b3-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="da4b3-113">Pravila za otklanjanje poteškoća</span><span class="sxs-lookup"><span data-stu-id="da4b3-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="da4b3-114">Da biste e-poštu (Exchange online) zaštitili od pristupa neusklađenih uređaja, oba dokumenta moraju se slijediti:</span><span class="sxs-lookup"><span data-stu-id="da4b3-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="da4b3-115">Zaštita pristupa e-pošti s uređaja pomoću EAS-a</span><span class="sxs-lookup"><span data-stu-id="da4b3-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="da4b3-116">Zaštita pristupa e-pošti s uređaja pomoću modernih klijenata za provjeru autentičnosti kao što je Outlook</span><span class="sxs-lookup"><span data-stu-id="da4b3-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)