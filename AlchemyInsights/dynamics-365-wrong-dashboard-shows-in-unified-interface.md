---
title: Dynamics 365-pogrešna nadzorna ploča prikazuje u sustavu Dynamics 365 objedinjeno sučelje
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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528543"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="c118d-102">Pogrešna nadzorna ploča prikazuje se u sustavu Dynamics 365 objedinjeno sučelje</span><span class="sxs-lookup"><span data-stu-id="c118d-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="c118d-103">Postoji nekoliko razloga zašto biste mogli vidjeti drugačiju nadzornu ploču od one koju očekujete:</span><span class="sxs-lookup"><span data-stu-id="c118d-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="c118d-104">Korisnik je postavio zadanu nadzornu ploču korisnika</span><span class="sxs-lookup"><span data-stu-id="c118d-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="c118d-105">Obično možete identificirati zadanu korisničku nadzornu ploču ako se **skup kao zadani** gumb ne pojavi na naredbenoj traci nadzorne ploče.</span><span class="sxs-lookup"><span data-stu-id="c118d-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="c118d-106">Zadana nadzorna ploča korisnika nadjačat će sve ostale zadane nadzorne ploče, čak i ako korisnikova zadana nadzorna ploča nije u trenutnoj aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="c118d-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="c118d-107">Za poništavanje postavljanja zadane nadzorne ploče koristite sljedeće zaobilazno rješenje.</span><span class="sxs-lookup"><span data-stu-id="c118d-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="c118d-108">Stvorite novu osobnu nadzornu ploču.</span><span class="sxs-lookup"><span data-stu-id="c118d-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="c118d-109">Postavite tu novu nadzornu ploču kao zadani korisnik.</span><span class="sxs-lookup"><span data-stu-id="c118d-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="c118d-110">Izbriši tu nadzornu ploču.</span><span class="sxs-lookup"><span data-stu-id="c118d-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="c118d-111">Nadzorna ploča postavljena je na karti web-mjesta</span><span class="sxs-lookup"><span data-stu-id="c118d-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="c118d-112">Možda ste postavili zadanu nadzornu ploču organizacije odabirom nadzorne ploče i odabirom opcije "Postavi kao zadano" pod "Prilagodi sustav".</span><span class="sxs-lookup"><span data-stu-id="c118d-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="c118d-113">No, nadzorna ploča definirana u dizajneru web-mjesta imat će prednost nad ovom nadzornom pločom ako korisnik ima pristup njemu.</span><span class="sxs-lookup"><span data-stu-id="c118d-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="c118d-114">Da bi korisnici vidjeli nadzornu ploču koju ste postavili kao zadanu organizaciju, možete:</span><span class="sxs-lookup"><span data-stu-id="c118d-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="c118d-115">Postavite tu nadzornu ploču na web-mjestu</span><span class="sxs-lookup"><span data-stu-id="c118d-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="c118d-116">Uklanjanje pristupa definiranoj nadzornoj ploči web-mjesta za te korisnike</span><span class="sxs-lookup"><span data-stu-id="c118d-116">Remove access to the sitemap defined dashboard for those users</span></span>
