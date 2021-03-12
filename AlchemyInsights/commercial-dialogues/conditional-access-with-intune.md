---
title: Korištenje uvjetnog pristupa pomoću aplikacije Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743682"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="b5afb-102">Korištenje uvjetnog pristupa pomoću aplikacije Intune</span><span class="sxs-lookup"><span data-stu-id="b5afb-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="b5afb-103">Korištenje uvjetnog pristupa pomoću aplikacije Intune zahtijeva tri koraka:</span><span class="sxs-lookup"><span data-stu-id="b5afb-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="b5afb-104">Stvaranje pravilnika o usklađenosti za definiranje postavki koje je potrebno ispuniti prije nego što se uređaj smatra sukladnim. Na primjer, uređaj mora imati PIN od najmanje 6 znamenki prije nego što se smatra sukladnim.</span><span class="sxs-lookup"><span data-stu-id="b5afb-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="b5afb-105">Stvorite pravilnik o uvjetnom pristupu koji definira resurse zaštićene i koje uvjete morate ispuniti da biste pristupili tim resursima. Na primjer, uređaj mora biti usklađen prije pristupanja korporativnom e-pošti.</span><span class="sxs-lookup"><span data-stu-id="b5afb-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="b5afb-106">Provjerite jesu li pravila usklađivanja i pravila uvjetnog pristupa usmjerena na željene grupe korisnika. To može zahtijevati stvaranje određenih grupa korisnika u servisu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b5afb-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="b5afb-107">Dodatne informacije...</span><span class="sxs-lookup"><span data-stu-id="b5afb-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
