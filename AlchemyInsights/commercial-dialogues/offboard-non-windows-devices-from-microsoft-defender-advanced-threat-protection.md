---
title: Offboard ne-Windows uređaji iz programa Microsoft Defender Napredna zaštita od prijetnji (ATP)
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
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743622"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="6ad93-102">Offboard ne-Windows uređaji iz programa Microsoft Defender Napredna zaštita od prijetnji (ATP)</span><span class="sxs-lookup"><span data-stu-id="6ad93-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="6ad93-103">Evo i kako:</span><span class="sxs-lookup"><span data-stu-id="6ad93-103">Here's how:</span></span>

1. <span data-ttu-id="6ad93-104">Slijedite dokumentaciju drugih proizvođača za prekid povezivanja rješenja drugog proizvođača iz programa Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="6ad93-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="6ad93-105">U odjeljku klijent za Azure Active Directory uklonite dozvole za rješenje drugog proizvođača:</span><span class="sxs-lookup"><span data-stu-id="6ad93-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="6ad93-106">Prijavite se na [portal Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="6ad93-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="6ad93-107">Odaberite **sve servise**  >  **Azure Active Directory**  >  **Enterprise aplikacije**.</span><span class="sxs-lookup"><span data-stu-id="6ad93-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="6ad93-108">Odaberite aplikaciju koju želite skinuti s ploče.</span><span class="sxs-lookup"><span data-stu-id="6ad93-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="6ad93-109">Odaberite **Izbriši**.</span><span class="sxs-lookup"><span data-stu-id="6ad93-109">Select **Delete**.</span></span>

<span data-ttu-id="6ad93-110">Dodatne informacije potražite u članku [off Board ne-Windows uređajima](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="6ad93-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
