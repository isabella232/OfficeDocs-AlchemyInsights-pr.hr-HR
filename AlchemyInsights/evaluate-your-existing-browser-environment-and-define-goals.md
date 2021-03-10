---
title: Vrednovanje postojećeg okruženja preglednika i definiranje ciljeva
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692715"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="38d03-102">Vrednovanje postojećeg okruženja preglednika i definiranje ciljeva</span><span class="sxs-lookup"><span data-stu-id="38d03-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="38d03-103">Uzimanje vremena da biste razumjeli vašu postojeću državu preglednika i projekt Vision osiguravaju da su svi dionici projekta usklađeni i da rade prema istom cilju.</span><span class="sxs-lookup"><span data-stu-id="38d03-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="38d03-104">Slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="38d03-104">Follow these steps:</span></span>

1. <span data-ttu-id="38d03-105">Definiranje sadašnjeg stanja.</span><span class="sxs-lookup"><span data-stu-id="38d03-105">Define your current state.</span></span> <span data-ttu-id="38d03-106">Razmotrite sljedeće mogućnosti:</span><span class="sxs-lookup"><span data-stu-id="38d03-106">Consider the following:</span></span>
- <span data-ttu-id="38d03-107">Koji su preglednici trenutno razmješteni u vašem okruženju?</span><span class="sxs-lookup"><span data-stu-id="38d03-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="38d03-108">Koji je preglednik postavljen kao zadani preglednik?</span><span class="sxs-lookup"><span data-stu-id="38d03-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="38d03-109">Trebate li koristiti Internet Explorer za neke aplikacije?</span><span class="sxs-lookup"><span data-stu-id="38d03-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="38d03-110">Koristite li popis web-mjesta Enterprise mode da biste konfigurirali Internet Explorer danas?</span><span class="sxs-lookup"><span data-stu-id="38d03-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="38d03-111">Koje platforme OS-a, kao što su Windows 10 i macOS, podržava vaše okruženje?</span><span class="sxs-lookup"><span data-stu-id="38d03-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="38d03-112">Koji Alati za upravljanje koristite za upravljanje preglednikom?</span><span class="sxs-lookup"><span data-stu-id="38d03-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="38d03-113">Tko je odgovoran za konfiguraciju i upravljanje preglednikom?</span><span class="sxs-lookup"><span data-stu-id="38d03-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="38d03-114">Koji je postupak za provjeru kompatibilnosti preglednika?</span><span class="sxs-lookup"><span data-stu-id="38d03-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="38d03-115">Definirajte ciljeve za implementaciju.</span><span class="sxs-lookup"><span data-stu-id="38d03-115">Define the goals for your deployment.</span></span> <span data-ttu-id="38d03-116">Imajte na umu sljedeće:</span><span class="sxs-lookup"><span data-stu-id="38d03-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="38d03-117">Želite li [postaviti Microsoft Edge kao zadani preglednik](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span><span class="sxs-lookup"><span data-stu-id="38d03-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="38d03-118">Želite li sakriti naslijeđenu verziju sustava Microsoft Edge ili [je želite ostaviti dostupnom korisnicima](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span><span class="sxs-lookup"><span data-stu-id="38d03-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="38d03-119">Kako ćete [konfigurirati Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span><span class="sxs-lookup"><span data-stu-id="38d03-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="38d03-120">Koje su značajke kritične za konfiguriranje kao dio početne implementacije?</span><span class="sxs-lookup"><span data-stu-id="38d03-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="38d03-121">Koji je postupak za rješavanje svih identififikog problema s kompatibilnošću ili konfiguracijom?</span><span class="sxs-lookup"><span data-stu-id="38d03-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="38d03-122">Razumijevanje preduvjeta za značajke koje možda želite koristiti, primjerice:</span><span class="sxs-lookup"><span data-stu-id="38d03-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="38d03-123">Čuvar aplikacije programa Windows Defender</span><span class="sxs-lookup"><span data-stu-id="38d03-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="38d03-124">Način rada u pregledniku Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="38d03-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="38d03-125">Provjera autentičnosti i sinkronizacija</span><span class="sxs-lookup"><span data-stu-id="38d03-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="38d03-126">Kada završite s ovim koracima, spremni ste početi planirati strategiju implementacije.</span><span class="sxs-lookup"><span data-stu-id="38d03-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
