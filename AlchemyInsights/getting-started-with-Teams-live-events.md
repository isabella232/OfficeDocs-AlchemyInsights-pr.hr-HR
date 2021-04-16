---
title: Početak rada s događajima uživo aplikacije Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811952"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="81dbf-102">Početak rada s događajima uživo aplikacije Teams</span><span class="sxs-lookup"><span data-stu-id="81dbf-102">Getting started with Teams live events</span></span>

<span data-ttu-id="81dbf-103">Događaji uživo aplikacije Teams predstavljaju proširenje sastanaka u aplikaciji Teams koji vam omogućuju zakazivanje i stvaranje događaja koji se prenose većim internetskim publikama.</span><span class="sxs-lookup"><span data-stu-id="81dbf-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="81dbf-104">Da biste stvorili događaj uživo, morat ćete učiniti sljedeće:</span><span class="sxs-lookup"><span data-stu-id="81dbf-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="81dbf-105">Najprije provjerite jesu li događaji uživo u aplikaciji Teams [dostupni u vašoj državi i regiji;](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability) Događaji uživo još nisu podržani u nekim državama.</span><span class="sxs-lookup"><span data-stu-id="81dbf-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="81dbf-106">Ako ste dodijelili licence i postavili pravilnike, ali i dalje ne možete stvoriti događaj u aplikaciji Teams Live, vjerojatno ste u državi ili regiji u kojoj događaji uživo još nisu dostupni.</span><span class="sxs-lookup"><span data-stu-id="81dbf-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="81dbf-107">Imajte [Licenca za Office 365 Enterprise E1, E3 ili E5 ili licenca za Office 365 A3 ili A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="81dbf-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="81dbf-108">**Napomena**: zbog porasta korištenja aplikacije Teams, kada korisniku dodijelite licencu aplikacije Teams, može proći do 24 sata prije no što se program za njega potpuno postavi.</span><span class="sxs-lookup"><span data-stu-id="81dbf-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="81dbf-109">Do tada mu nećete moći dodjeljivati pravilnike aplikacije Teams, a on možda neće imati pristup određenim značajkama aplikacije Teams kao što su pozivi i audiokonferencije.</span><span class="sxs-lookup"><span data-stu-id="81dbf-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="81dbf-110">Dozvola za [stvaranje događaja uživo u centru za administratore aplikacije Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="81dbf-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="81dbf-111">Dozvola za [stvaranje događaja uživo u servisu Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (za događaja stvorene pomoću vanjske aplikacije ili uređaja za emitiranje).</span><span class="sxs-lookup"><span data-stu-id="81dbf-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="81dbf-112">Puno timsko članstvo u tvrtki ili ustanovi (korisnik ne može biti gost niti potjecati iz druge tvrtke ili ustanove).</span><span class="sxs-lookup"><span data-stu-id="81dbf-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="81dbf-113">Zakazivanje privatnih sastanaka, zajedničko korištenje radnih površina dijeljenje IP videozapisa uključeno u pravilniku za sastanke aplikacije Teams.</span><span class="sxs-lookup"><span data-stu-id="81dbf-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="81dbf-114">[Najbolje prakse](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) za događaje uživo u aplikaciji Teams.</span><span class="sxs-lookup"><span data-stu-id="81dbf-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="81dbf-115">Za dodatne informacije pogledajte [Početak rada s događajima uživo aplikacije Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="81dbf-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>