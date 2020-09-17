---
title: Uvjetni pristup pomoću aplikacije Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807651"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="ae99f-102">Uvjetni pristup pomoću aplikacije Intune</span><span class="sxs-lookup"><span data-stu-id="ae99f-102">Conditional Access with Intune</span></span>

<span data-ttu-id="ae99f-103">Korištenje  **uvjetnog pristupa**  pomoću aplikacije Intune zahtijeva tri koraka:</span><span class="sxs-lookup"><span data-stu-id="ae99f-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="ae99f-104">Stvaranje  **pravilnika o usklađenosti**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) za definiranje postavki koje je potrebno ispuniti prije nego što se uređaj smatra sukladnim.</span><span class="sxs-lookup"><span data-stu-id="ae99f-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="ae99f-105">Na primjer, uređaj mora imati PIN od najmanje 6 znamenki prije nego što se smatra sukladnim.</span><span class="sxs-lookup"><span data-stu-id="ae99f-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="ae99f-106">Stvorite **pravilnik o uvjetnom pristupu**  koji definira resurse zaštićene i koje uvjete morate ispuniti da biste pristupili tim resursima.</span><span class="sxs-lookup"><span data-stu-id="ae99f-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="ae99f-107">[Na primjer,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  uređaj mora biti usklađen prije pristupanja korporativnom e-pošti.</span><span class="sxs-lookup"><span data-stu-id="ae99f-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="ae99f-108">Provjerite jesu li **pravila usklađivanja**  i pravila  **uvjetnog pristupa**  usmjerena na željene grupe korisnika.</span><span class="sxs-lookup"><span data-stu-id="ae99f-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="ae99f-109">To može zahtijevati stvaranje određenih grupa korisnika u servisu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ae99f-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="ae99f-110">**Korisne veze:**</span><span class="sxs-lookup"><span data-stu-id="ae99f-110">**Helpful links:**</span></span>

[<span data-ttu-id="ae99f-111">Pregled usklađenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="ae99f-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="ae99f-112">Otklanjanje poteškoća sa com</span><span class="sxs-lookup"><span data-stu-id="ae99f-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="ae99f-113">Pravilnik o otklanjanju poteškoća</span><span class="sxs-lookup"><span data-stu-id="ae99f-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="ae99f-114">Da biste zaštitili e-poštu (Exchange Online) iz programa Access prema nesukladnim uređajima, moraju se pratiti oba dokumenta:</span><span class="sxs-lookup"><span data-stu-id="ae99f-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="ae99f-115">Zaštita pristupa e-pošti s uređaja pomoću servisa EAS</span><span class="sxs-lookup"><span data-stu-id="ae99f-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="ae99f-116">Zaštita pristupa e-pošti s uređaja pomoću modernih klijenata za provjeru autentičnosti kao što je Outlook</span><span class="sxs-lookup"><span data-stu-id="ae99f-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)