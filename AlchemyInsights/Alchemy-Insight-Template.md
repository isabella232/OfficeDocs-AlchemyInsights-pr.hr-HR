---
title: isto kao i naziv datoteke je najbolje
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/15/2019
ms.locfileid: "35800037"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="df882-102">Potrebna Alkemija zaglavlje H1, H2's ne radi.</span><span class="sxs-lookup"><span data-stu-id="df882-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="df882-103">Najbolje prakse i smjernice za alhemiju autoriranje:</span><span class="sxs-lookup"><span data-stu-id="df882-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="df882-104">**Ne gnijezdi alhemije uvide u mapama**-to će razbiti strukturu URL-a.</span><span class="sxs-lookup"><span data-stu-id="df882-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="df882-105">Mi smo u potrazi za popravak ovo.</span><span class="sxs-lookup"><span data-stu-id="df882-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="df882-106">Datoteke u mapi **Alchemyin,** trebali bi imati mala imena s crtama za razmake.</span><span class="sxs-lookup"><span data-stu-id="df882-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="df882-107">***kako-omogućiti-suđenje-čekanje***.</span><span class="sxs-lookup"><span data-stu-id="df882-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="df882-108">Uključi ID pravila ili ID polja s [portala alhemije partnera](https://alchemyportal.azurewebsites.net) u polje MS. Prilagođeno.</span><span class="sxs-lookup"><span data-stu-id="df882-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="df882-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="df882-109">ex.</span></span> <span data-ttu-id="df882-110">***MS. običaj: 100021***</span><span class="sxs-lookup"><span data-stu-id="df882-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="df882-111">Koristite ostatak metapodataka na vrhu ove datoteke kao predložak.</span><span class="sxs-lookup"><span data-stu-id="df882-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="df882-112">Na [portalu alhemski partner](https://alchemyportal.azurewebsites.net)pomaknite se do sekcije **Kupac uvida u naslov:** i koristite to kao početnu točku za vaš u</span><span class="sxs-lookup"><span data-stu-id="df882-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="df882-113">Alhemija uvidi mora imati samo jedan H1 na vrhu ili će razbiti u proizvodnji.</span><span class="sxs-lookup"><span data-stu-id="df882-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="df882-114">H2s Nemojte tako koristiti **podebljane** ili druge konvencije da biste označili odvojene sekcije.</span><span class="sxs-lookup"><span data-stu-id="df882-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="df882-115">Zatim ispunite tijelo tekst pomoću skice materijala u odjeljku klijent uvidi na stranici alhemija pravila</span><span class="sxs-lookup"><span data-stu-id="df882-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="df882-116">Popisi s grafičkim oznakama su u redu</span><span class="sxs-lookup"><span data-stu-id="df882-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="df882-117">Numerirani popisi previše</span><span class="sxs-lookup"><span data-stu-id="df882-117">Numbered lists too</span></span>
    1. <span data-ttu-id="df882-118">**Bold** i *kurziv* su u redu</span><span class="sxs-lookup"><span data-stu-id="df882-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="df882-119">Linkovi uvijek moraju biti **"veze na web"/vanjski** ili **Deep-linkovi na elemente korisničkog sučelja**, a ne interne veze.</span><span class="sxs-lookup"><span data-stu-id="df882-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="df882-120">Slike nisu službeno podržane u ovom trenutku, ali je na planu.</span><span class="sxs-lookup"><span data-stu-id="df882-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="df882-121">A ovo je stvarno već malo predugo.</span><span class="sxs-lookup"><span data-stu-id="df882-121">And this is really already a bit too long.</span></span> <span data-ttu-id="df882-122">Najbolja praksa je oko 400 znakova---------------------------------</span><span class="sxs-lookup"><span data-stu-id="df882-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="df882-123">Kada vaš sadržaj bude spreman, povucite ga u živu granu.</span><span class="sxs-lookup"><span data-stu-id="df882-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="df882-124">Zatim idite na [portal alhemije partner](https://alchemyportal.azurewebsites.net) i unesite naziv datoteke u polje URL.</span><span class="sxs-lookup"><span data-stu-id="df882-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 