---
title: Politika zaštite aplikacija
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423333"
---
# <a name="application-protection-policy"></a><span data-ttu-id="10cc9-102">Politika zaštite aplikacija</span><span class="sxs-lookup"><span data-stu-id="10cc9-102">Application protection policy</span></span>

<span data-ttu-id="10cc9-103">Ako ste novi u pravilima o zaštiti aplikacija (APP), pogledajte [pregled pravila zaštite aplikacija](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="10cc9-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="10cc9-104">Da biste počeli koristiti APP, [pročitajte članak Kako izraditi i dodijeliti pravila zaštite aplikacija](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="10cc9-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="10cc9-105">Zahtjevi politike zaštite aplikacija:</span><span class="sxs-lookup"><span data-stu-id="10cc9-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="10cc9-106">Korisnik ima Intune ili EMS licencu.</span><span class="sxs-lookup"><span data-stu-id="10cc9-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="10cc9-107">Korisnik pripada grupi koju ciljaju pravila zaštite aplikacija.</span><span class="sxs-lookup"><span data-stu-id="10cc9-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="10cc9-108">Samo je jedan korporativni korisnik prijavljen u zaštićene aplikacije na uređaju.</span><span class="sxs-lookup"><span data-stu-id="10cc9-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="10cc9-109">Aplikacija je implementirala [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="10cc9-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="10cc9-110">Popis aplikacija koje podržavaju SDK potražite u odjeljku [Aplikacije zaštićene Microsoft Intune .](https://docs.microsoft.com/intune/apps-supported-intune-apps)</span><span class="sxs-lookup"><span data-stu-id="10cc9-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="10cc9-111">Pravila se primjenjuju nakon što korisnik koji ispunjava gore navedene zahtjeve potpiše aplikaciju s omogućenom Intune SDK-om.</span><span class="sxs-lookup"><span data-stu-id="10cc9-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="10cc9-112">Najjednostavniji način za utvrđivanje primjenjuje li se pravilo tako da korisnik postavi pin u pravilima.</span><span class="sxs-lookup"><span data-stu-id="10cc9-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="10cc9-113">Dodatne informacije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="10cc9-113">For more information, see:</span></span>

[<span data-ttu-id="10cc9-114">Najčešća pitanja o otklanjanju poteškoća s APP/MAM-om</span><span class="sxs-lookup"><span data-stu-id="10cc9-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="10cc9-115">Kako provjeriti postavljanje pravila zaštite aplikacija</span><span class="sxs-lookup"><span data-stu-id="10cc9-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="10cc9-116">Objašnjenje vremena isporuke pravila zaštite aplikacija</span><span class="sxs-lookup"><span data-stu-id="10cc9-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="10cc9-117">Kako pratiti pravila zaštite aplikacija</span><span class="sxs-lookup"><span data-stu-id="10cc9-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)