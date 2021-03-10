---
title: Otkrivanje web-mjesta
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
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692671"
---
# <a name="do-site-discovery"></a><span data-ttu-id="75661-102">Otkrivanje web-mjesta</span><span class="sxs-lookup"><span data-stu-id="75661-102">Do site discovery</span></span>

<span data-ttu-id="75661-103">Ako vaša tvrtka ili ustanova još uvijek koristi naslijeđene web-aplikacije i planira koristiti način rada u pregledniku Internet Explorer (što većina kupaca radi), trebali biste učiniti dodatna otkrića web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="75661-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="75661-104">**Već ste implementirali stariju verziju sustava Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="75661-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="75661-105">Ako ste već konfigurirali popis web-mjesta tvrtke da funkcionira za naslijeđenu verziju sustava Microsoft Edge, otkriće web-mjesta gotovo je dovršeno.</span><span class="sxs-lookup"><span data-stu-id="75661-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="75661-106">Možda ćete morati dodati neutralna web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="75661-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="75661-107">Neutralna web-mjesta obično su web-mjesta koja sadrže jedinstvenu prijavu (SSO).</span><span class="sxs-lookup"><span data-stu-id="75661-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="75661-108">Ako odete na neutralno web-mjesto iz programa Microsoft Edge, želite biti autentificiraj u pregledniku Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="75661-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="75661-109">Ako u načinu rada Internet Explorera odete na neutralno web-mjesto, u načinu rada u pregledniku Internet Explorer želite biti autentificiraj.</span><span class="sxs-lookup"><span data-stu-id="75661-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="75661-110">Odredite bilo koje SSO ili druga neutralna web-mjesta koja koristite i dodajte ih na popis web-mjesta tvrtke.</span><span class="sxs-lookup"><span data-stu-id="75661-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="75661-111">**Internet Explorer zadani je preglednik**</span><span class="sxs-lookup"><span data-stu-id="75661-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="75661-112">Ako trenutno koristite Internet Explorer, možda nećete znati koje su web-mjesta nadogradili na moderne web-standarde i za koje je i dalje potreban Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="75661-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="75661-113">Te web-mjesta želite pronaći i dodati na popis Enterprise web-mjesta da biste mogli koristiti način rada u pregledniku Internet Explorer samo za ta web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="75661-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="75661-114">[Otkriće web-mjesta Enterprise](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) otkriva web-mjesta koja možda trebaju način rada preglednika Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="75661-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="75661-115">Može prikupljati podatke na računalima sa sustavom Windows Internet Explorer 8 putem preglednika Internet Explorer 11 u sustavima Windows 10, Windows 8,1 ili Windows 7.</span><span class="sxs-lookup"><span data-stu-id="75661-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="75661-116">**Analiziranje podataka**</span><span class="sxs-lookup"><span data-stu-id="75661-116">**Analyze the data**</span></span>

<span data-ttu-id="75661-117">Kada prikupite podatke web-mjesta, preporučujemo sljedeći postupak u četiri koraka radi analize podataka:</span><span class="sxs-lookup"><span data-stu-id="75661-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="75661-118">Sortirajte podatke prema domeni, a zatim prema URL-u.</span><span class="sxs-lookup"><span data-stu-id="75661-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="75661-119">Definiranje granica aplikacije za konfiguriranje načina rada u pregledniku Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="75661-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="75661-120">Želite uvrstiti sva web-mjesta i web-kontrole koje definiraju aplikaciju, ali ne želite uvrstiti dodatna web-mjesta i kontrole.</span><span class="sxs-lookup"><span data-stu-id="75661-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="75661-121">Neka web-mjesta mogu biti jednostavna kao i *https://contoso.com/app1* dok bi drugi mogli zahtijevati definiranje više web-mjesta i stranica.</span><span class="sxs-lookup"><span data-stu-id="75661-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="75661-122">Testirajte aplikaciju da biste potvrdili da ne funkcionira u urođenom.</span><span class="sxs-lookup"><span data-stu-id="75661-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="75661-123">Mnoga će web-mjesta ponuditi moderan sadržaj kada otkriju moderan preglednik i nude samo naslijeđeni sadržaj kada otkriju Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="75661-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="75661-124">Dodajte aplikaciju na popis web-mjesta tvrtke ako ne uspije testirati.</span><span class="sxs-lookup"><span data-stu-id="75661-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="75661-125">Kao najbolju praksu grupirajte sva web-mjesta koja sadrže aplikaciju.</span><span class="sxs-lookup"><span data-stu-id="75661-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="75661-126">Na taj način, kada nadogradite aplikaciju, lakše je ukloniti cijelo web-mjesto iz načina rada Internet Explorer i početi koristiti moderan preglednik za tu aplikaciju.</span><span class="sxs-lookup"><span data-stu-id="75661-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="75661-127">Kada završite s otkrivanjem web-mjesta i analizirali ste podatke, spremni ste početi gledati strategiju kanala.</span><span class="sxs-lookup"><span data-stu-id="75661-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

