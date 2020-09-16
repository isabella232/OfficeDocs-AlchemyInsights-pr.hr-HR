---
title: Pravilnik o zaštiti aplikacija
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716885"
---
# <a name="application-protection-policy"></a><span data-ttu-id="7e8cf-102">Pravilnik o zaštiti aplikacija</span><span class="sxs-lookup"><span data-stu-id="7e8cf-102">Application protection policy</span></span>

<span data-ttu-id="7e8cf-103">Ako ste novi pravilnik o zaštiti aplikacija (aplikacija), pogledajte [Pregled pravilnika o zaštiti aplikacija](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="7e8cf-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="7e8cf-104">Da biste počeli koristiti aplikaciju, pročitajte članak [Stvaranje i dodjela pravilnika o zaštiti aplikacija](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="7e8cf-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="7e8cf-105">Preduvjeti pravilnika o zaštiti aplikacija:</span><span class="sxs-lookup"><span data-stu-id="7e8cf-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="7e8cf-106">Korisnik ima licencu za Intune ili EMS.</span><span class="sxs-lookup"><span data-stu-id="7e8cf-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="7e8cf-107">Korisnik pripada grupi ciljanu u pravilima zaštite aplikacija.</span><span class="sxs-lookup"><span data-stu-id="7e8cf-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="7e8cf-108">U zaštićenim aplikacijama na uređaju potpisan je samo jedan korporacijski korisnik.</span><span class="sxs-lookup"><span data-stu-id="7e8cf-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="7e8cf-109">Aplikacija je implementirala [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="7e8cf-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="7e8cf-110">Popis aplikacija koje podržavaju SDK potražite u [članku Microsoft Intune Protected Apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="7e8cf-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="7e8cf-111">Pravila se primjenjuju nakon što korisnik koji udovoljava navedenim zahtjevima potpiše u aplikaciju Intune SDK koja je omogućena.</span><span class="sxs-lookup"><span data-stu-id="7e8cf-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="7e8cf-112">Najlakše ćete odrediti primjenjuje li se pravilo tako da korisnik postavi PIN u pravilniku.</span><span class="sxs-lookup"><span data-stu-id="7e8cf-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="7e8cf-113">Dodatne informacije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="7e8cf-113">For more information, see:</span></span>

[<span data-ttu-id="7e8cf-114">Najčešća pitanja o otklanjanju poteškoća s aplikacijom/MAM</span><span class="sxs-lookup"><span data-stu-id="7e8cf-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="7e8cf-115">Provjera valjanosti postavljanja pravilnika o zaštiti aplikacija</span><span class="sxs-lookup"><span data-stu-id="7e8cf-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="7e8cf-116">Objašnjenje vremena isporuke pravilnika o zaštiti aplikacija</span><span class="sxs-lookup"><span data-stu-id="7e8cf-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="7e8cf-117">Praćenje pravilnika o zaštiti aplikacija</span><span class="sxs-lookup"><span data-stu-id="7e8cf-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)