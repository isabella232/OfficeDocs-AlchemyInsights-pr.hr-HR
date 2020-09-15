---
title: isto kao što je naziv datoteke najbolji
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664126"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="fb11d-102">"Required"</span><span class="sxs-lookup"><span data-stu-id="fb11d-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="fb11d-103">Najbolje prakse i smjernice za autorizaciju:</span><span class="sxs-lookup"><span data-stu-id="fb11d-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="fb11d-104">**Ne gnijezdite uvide u mapama u mapi**-to će prekinuti strukturu URL-a.</span><span class="sxs-lookup"><span data-stu-id="fb11d-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="fb11d-105">Traћimo da popravimo ovo.</span><span class="sxs-lookup"><span data-stu-id="fb11d-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="fb11d-106">Datoteke u mapi **alfihuspoznaje** trebale bi imati slova s malim slovima s crtima za Spaces ex.</span><span class="sxs-lookup"><span data-stu-id="fb11d-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="fb11d-107">***Kako-to-ovlastiti-spor-čekanje***.</span><span class="sxs-lookup"><span data-stu-id="fb11d-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="fb11d-108">[U polje](https://alchemyportal.azurewebsites.net) MS. Custom unesite ID pravila ili ID narudžbe.</span><span class="sxs-lookup"><span data-stu-id="fb11d-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="fb11d-109">primjerice.</span><span class="sxs-lookup"><span data-stu-id="fb11d-109">ex.</span></span> <span data-ttu-id="fb11d-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="fb11d-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="fb11d-111">Koristite ostale metapodatke pri vrhu ove datoteke u obliku predloška.</span><span class="sxs-lookup"><span data-stu-id="fb11d-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="fb11d-112">Na [portalu za partnere Alsimija](https://alchemyportal.azurewebsites.net)pomaknite se prema dolje do odjeljka **naslov korisničkog privida:** i koristite ga kao početnu točku za svoj H1 Title za uvid.</span><span class="sxs-lookup"><span data-stu-id="fb11d-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="fb11d-113">Alimija uvide mora imati samo jedan H1 na vrhu ili će se probiti u proizvodnji.</span><span class="sxs-lookup"><span data-stu-id="fb11d-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="fb11d-114">H2s ne prikazirajte tako da koristite **podebljano** ili druge konvencije da biste označili odvojene sekcije.</span><span class="sxs-lookup"><span data-stu-id="fb11d-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="fb11d-115">Zatim unesite tekst tijela pomoću skice materijala u odjeljku statistika korisnika na stranici pravila Alfala</span><span class="sxs-lookup"><span data-stu-id="fb11d-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="fb11d-116">Popisi s grafičkim oznakama su u redu</span><span class="sxs-lookup"><span data-stu-id="fb11d-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="fb11d-117">Numerirani popisi previše</span><span class="sxs-lookup"><span data-stu-id="fb11d-117">Numbered lists too</span></span>
    1. <span data-ttu-id="fb11d-118">**Podebljano** i *kurziv* su-u redu</span><span class="sxs-lookup"><span data-stu-id="fb11d-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="fb11d-119">Veze uvijek moraju biti **"veze na web"/vanjske** ili **duboke veze na elemente korisničkog sučelja**, a ne interne veze.</span><span class="sxs-lookup"><span data-stu-id="fb11d-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="fb11d-120">Slike trenutno nisu podržane, ali se nalaze na putokaz.</span><span class="sxs-lookup"><span data-stu-id="fb11d-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="fb11d-121">I ovo je već već malo predugačko.</span><span class="sxs-lookup"><span data-stu-id="fb11d-121">And this is really already a bit too long.</span></span> <span data-ttu-id="fb11d-122">Najbolja praksa iznosi oko 400 znakova---------------------------------</span><span class="sxs-lookup"><span data-stu-id="fb11d-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="fb11d-123">Kada sadržaj bude spreman, povucite ga u Live Branch.</span><span class="sxs-lookup"><span data-stu-id="fb11d-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="fb11d-124">Zatim otvorite [portal za partnere Alfimije](https://alchemyportal.azurewebsites.net) i unesite naziv datoteke u polje URL.</span><span class="sxs-lookup"><span data-stu-id="fb11d-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 