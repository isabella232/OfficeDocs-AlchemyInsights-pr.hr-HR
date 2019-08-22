---
title: Dynamics 365 - pogrešan nadzorne ploče prikazuje u sučelju Objedinjena Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528543"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="73b5d-102">Prikazuje pogrešne nadzorne ploče u sučelju Objedinjena Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="73b5d-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="73b5d-103">Postoji nekoliko razloga zašto možda vidjeti drugu tablu od očekujete:</span><span class="sxs-lookup"><span data-stu-id="73b5d-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="73b5d-104">Korisnik je postaviti zadane nadzorne ploče korisnika</span><span class="sxs-lookup"><span data-stu-id="73b5d-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="73b5d-105">Obično možete identificirati korisnika zadanu nadzornu ploču postavite ako **Postavite kao zadani** gumb Pokaži u naredbenoj traci nadzorne ploče.</span><span class="sxs-lookup"><span data-stu-id="73b5d-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="73b5d-106">Podrazumevanu kontrolnu tablu korisnika nadjačat će sve druge zadane nadzorne ploče, čak i ako se zadane nadzorne ploče korisnika nije u trenutnom app.</span><span class="sxs-lookup"><span data-stu-id="73b5d-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="73b5d-107">Koristite sljedeće zaobilazno rješenje za unset njihove zadane nadzorne ploče.</span><span class="sxs-lookup"><span data-stu-id="73b5d-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="73b5d-108">Stvori novu nadzornu osobne.</span><span class="sxs-lookup"><span data-stu-id="73b5d-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="73b5d-109">Tu novu nadzornu ploču postavite kao zadani korisnik.</span><span class="sxs-lookup"><span data-stu-id="73b5d-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="73b5d-110">Izbrišite tu nadzornu ploču.</span><span class="sxs-lookup"><span data-stu-id="73b5d-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="73b5d-111">Nadzornu ploču postavite u na mapu lokacije</span><span class="sxs-lookup"><span data-stu-id="73b5d-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="73b5d-112">Možda ste postavili organizacije zadane nadzorne ploče odabirom nadzorne ploče i odabirom 'Postavi kao zadano' pod 'Prilagoditi sustav'.</span><span class="sxs-lookup"><span data-stu-id="73b5d-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="73b5d-113">Ali nadzorne ploče definirane u dizajneru karte web-mjesta će prednost nad nadzorna ploča, ako korisnik ima pristup.</span><span class="sxs-lookup"><span data-stu-id="73b5d-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="73b5d-114">Da bi korisnici vidjeli nadzornu ploču postavite kao zadanu organizaciji, možete je:</span><span class="sxs-lookup"><span data-stu-id="73b5d-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="73b5d-115">Postavite tu nadzornu ploču na mapu lokacije</span><span class="sxs-lookup"><span data-stu-id="73b5d-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="73b5d-116">Uklanjanje pristupa nadzorne ploče karte definiran za one korisnike</span><span class="sxs-lookup"><span data-stu-id="73b5d-116">Remove access to the sitemap defined dashboard for those users</span></span>
