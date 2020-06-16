---
title: rečeni kao ime datoteke je najbolji
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750962"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="1bcc1-102">"Obavezno Alkemija Zaglavlje H1, H2 ne rade."</span><span class="sxs-lookup"><span data-stu-id="1bcc1-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="1bcc1-103">Najbolje prakse i smjernice za autorstvo alkemije:</span><span class="sxs-lookup"><span data-stu-id="1bcc1-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="1bcc1-104">**Nemojte gnijezditi Alkemijske uvide u mape**- to će slomiti strukturu URL-a.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="1bcc1-105">Istražujemo popravljanje ovoga.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="1bcc1-106">Datoteke u mapi **AlchemyInsights** trebale bi imati mala imena datoteka s crticama za razmake ex.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="1bcc1-107">***kako-to- ovlastiti- sudska prijava- održavati se.***</span><span class="sxs-lookup"><span data-stu-id="1bcc1-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="1bcc1-108">U polje ms.custom uključite ID pravila ili ID kante s [portala Alkemije](https://alchemyportal.azurewebsites.net) partnera.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="1bcc1-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-109">ex.</span></span> <span data-ttu-id="1bcc1-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="1bcc1-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="1bcc1-111">Kao predložak koristite ostale metapodatke pri vrhu ove datoteke.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="1bcc1-112">Na [portalu Alkemijskih partnera](https://alchemyportal.azurewebsites.net)idite do odjeljka **Naslov uvida korisnika:** i upotrijebite je kao početnu točku za naslov H1 za uvid.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="1bcc1-113">Alkemija Insights mora imati samo jedan H1 na vrhu ili će razbiti u proizvodnji.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="1bcc1-114">H2s ne čine bilo tako koristiti **podebljano** ili druge konvencije za označavanje zasebnih sekcija.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="1bcc1-115">Zatim ispunite tekst tijela pomoću nacrta materijala u odjeljku Customer Insights na stranici Pravilo alkemije</span><span class="sxs-lookup"><span data-stu-id="1bcc1-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="1bcc1-116">Popisi s grafičkim oznakama su u redu</span><span class="sxs-lookup"><span data-stu-id="1bcc1-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="1bcc1-117">Numerirani popisi previše</span><span class="sxs-lookup"><span data-stu-id="1bcc1-117">Numbered lists too</span></span>
    1. <span data-ttu-id="1bcc1-118">**Podebljano** i *kurziv* su-ok</span><span class="sxs-lookup"><span data-stu-id="1bcc1-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="1bcc1-119">Linkovi bi uvijek trebali biti **"linkovi na web"/vanjski** ili **duboke veze na elemente korisničkog sučelja,** a ne interne veze.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="1bcc1-120">Slike trenutno nisu službeno podržane, ali su na planu.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="1bcc1-121">A ovo je već malo predugo.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-121">And this is really already a bit too long.</span></span> <span data-ttu-id="1bcc1-122">Najbolja praksa je oko 400 znakova ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="1bcc1-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="1bcc1-123">Nakon što je vaš sadržaj spreman, povucite ga na živu granu.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="1bcc1-124">Zatim idite na [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) i unesite naziv datoteke u polje URL-a.</span><span class="sxs-lookup"><span data-stu-id="1bcc1-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 