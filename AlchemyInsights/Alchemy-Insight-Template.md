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
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676525"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="43cd4-102">Obavezno Alkemija Zaglavlje H1, H2's ne rade.</span><span class="sxs-lookup"><span data-stu-id="43cd4-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="43cd4-103">Najbolje prakse i smjernice za alkemiju:</span><span class="sxs-lookup"><span data-stu-id="43cd4-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="43cd4-104">**Nemojte gnijezditi Alchemy Insights u mapama**- to će razbiti strukturu URL-a.</span><span class="sxs-lookup"><span data-stu-id="43cd4-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="43cd4-105">Tražimo da ovo popravimo.</span><span class="sxs-lookup"><span data-stu-id="43cd4-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="43cd4-106">Datoteke u mapi **AlchemyInsights trebale** bi imati male nazive datoteka s crticama za razmakex.</span><span class="sxs-lookup"><span data-stu-id="43cd4-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="43cd4-107">***kako-to-omogućiti-parnica-hold.***</span><span class="sxs-lookup"><span data-stu-id="43cd4-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="43cd4-108">Uključite ID pravila ili bucket S [portala Alchemy Partner](https://alchemyportal.azurewebsites.net) u polje ms.custom.</span><span class="sxs-lookup"><span data-stu-id="43cd4-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="43cd4-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="43cd4-109">ex.</span></span> <span data-ttu-id="43cd4-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="43cd4-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="43cd4-111">Ostale metapodatke pri vrhu ove datoteke koristite kao predložak.</span><span class="sxs-lookup"><span data-stu-id="43cd4-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="43cd4-112">Na [portalu Partner za alkemiju](https://alchemyportal.azurewebsites.net)idite na odjeljak **Naslov uvida korisnika:** i koristite to kao početnu točku za naslov H1 za uvid.</span><span class="sxs-lookup"><span data-stu-id="43cd4-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="43cd4-113">Alkemija Insights MORA imati samo jedan H1 na vrhu ili će razbiti u proizvodnji.</span><span class="sxs-lookup"><span data-stu-id="43cd4-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="43cd4-114">H2 s prikazom ni od njih koristite **podebljane** ili druge konvencije za označavanje zasebnih sekcija.</span><span class="sxs-lookup"><span data-stu-id="43cd4-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="43cd4-115">Zatim ispunite tijelo teksta pomoću skica materijala u odjeljku Uvidi korisnici na stranici Pravilo o upotrebi</span><span class="sxs-lookup"><span data-stu-id="43cd4-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="43cd4-116">Popisi s grafičkim oznakama su u redu</span><span class="sxs-lookup"><span data-stu-id="43cd4-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="43cd4-117">Numerirani popisi također</span><span class="sxs-lookup"><span data-stu-id="43cd4-117">Numbered lists too</span></span>
    1. <span data-ttu-id="43cd4-118">**Podebljano** i *kurziv* je u redu.</span><span class="sxs-lookup"><span data-stu-id="43cd4-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="43cd4-119">Linkovi bi uvijek trebali biti **"linkovi na web"/vanjske** ILI **dubinske veze na elemente korisničkog sučelja,** a ne interne veze.</span><span class="sxs-lookup"><span data-stu-id="43cd4-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="43cd4-120">Slike trenutno nisu službeno podržane, ali je na planu.</span><span class="sxs-lookup"><span data-stu-id="43cd4-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="43cd4-121">A ovo je stvarno već malo predugo.</span><span class="sxs-lookup"><span data-stu-id="43cd4-121">And this is really already a bit too long.</span></span> <span data-ttu-id="43cd4-122">Najbolja praksa je oko 400 znakova ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="43cd4-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="43cd4-123">Nakon što je vaš sadržaj spreman, povucite ga u živu granu.</span><span class="sxs-lookup"><span data-stu-id="43cd4-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="43cd4-124">Zatim idite na [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) i unesite naziv datoteke u polje URL-a.</span><span class="sxs-lookup"><span data-stu-id="43cd4-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 