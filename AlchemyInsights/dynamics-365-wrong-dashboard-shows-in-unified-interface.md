---
title: Dinamika 365 – pogrešna nadzorna ploča u sustavu Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711267"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="62541-102">Pogrešan prikaz nadzorne ploče u sustavu Dynamics 365 Unified Interface</span><span class="sxs-lookup"><span data-stu-id="62541-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="62541-103">Postoji nekoliko razloga zbog kojih možete vidjeti neku drugu nadzornu ploču od one koju očekujete:</span><span class="sxs-lookup"><span data-stu-id="62541-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="62541-104">Korisnik je postavio zadanu nadzornu ploču korisnika</span><span class="sxs-lookup"><span data-stu-id="62541-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="62541-105">Obično je moguće identificirati zadanu nadzornu ploču korisnika, ako se gumb **Postavi kao zadani** ne prikazuje na naredbenom traku nadzorne ploče.</span><span class="sxs-lookup"><span data-stu-id="62541-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="62541-106">Zadana nadzorna ploča korisnika nadjačat će sve druge zadane nadzorne ploče, čak i ako se zadana nadzorna ploča korisnika ne nalazi u aktualnoj aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="62541-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="62541-107">Da biste poništili zadanu nadzornu ploču, upotrijebite sljedeće zaobilazno rješenje.</span><span class="sxs-lookup"><span data-stu-id="62541-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="62541-108">Stvorite novu osobnu nadzornu ploču.</span><span class="sxs-lookup"><span data-stu-id="62541-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="62541-109">Postavite tu novu nadzornu ploču kao zadanu korisniku.</span><span class="sxs-lookup"><span data-stu-id="62541-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="62541-110">Izbrišite tu nadzornu ploču.</span><span class="sxs-lookup"><span data-stu-id="62541-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="62541-111">Nadzorna ploča postavljena je na web-stranici Sitemap</span><span class="sxs-lookup"><span data-stu-id="62541-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="62541-112">Možda ste postavili zadanu nadzornu ploču tvrtke ili ustanove tako da odaberete nadzornu ploču i odaberete "Postavi kao zadano" u odjeljku "Prilagodba sustava".</span><span class="sxs-lookup"><span data-stu-id="62541-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="62541-113">No nadzorna ploča definirana u dizajneru Sitemap imat će prednost nad tom nadzornom tabicom ako korisnik ima pristup.</span><span class="sxs-lookup"><span data-stu-id="62541-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="62541-114">Da bi korisnici mogli vidjeti nadzornu ploču koju ste postavili kao zadanu za tvrtku ili ustanovu, možete učiniti sljedeće:</span><span class="sxs-lookup"><span data-stu-id="62541-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="62541-115">Postavljanje nadzorne ploče u mapi Sitemap</span><span class="sxs-lookup"><span data-stu-id="62541-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="62541-116">Uklanjanje pristupa definiranoj nadzornoj ploči web-stranice za te korisnike</span><span class="sxs-lookup"><span data-stu-id="62541-116">Remove access to the sitemap defined dashboard for those users</span></span>
