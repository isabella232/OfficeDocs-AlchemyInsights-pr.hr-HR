---
title: isti kao naziv datoteke je najbolje
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
ms.openlocfilehash: ec979c2f2246fa06945b79bbb9348a7a57ad5180
ms.sourcegitcommit: b3cf5130ac8118f0fed66abe5286aa80ee91af52
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2019
ms.locfileid: "30683841"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="83293-102">Potrebna alkemiji zaglavlje H1, H2's ne rade.</span><span class="sxs-lookup"><span data-stu-id="83293-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="83293-103">Najbolje prakse i smjernice za autorizaciju alkemiji:</span><span class="sxs-lookup"><span data-stu-id="83293-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="83293-104">**Ugnijezditi alkemiji uvida u mapama**- će ovo prelomiti strukturu url.</span><span class="sxs-lookup"><span data-stu-id="83293-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="83293-105">Možemo traženu u popravljanju to.</span><span class="sxs-lookup"><span data-stu-id="83293-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="83293-106">Datoteke u mapi **AlchemyInsights** treba imati malo nazivi datoteka s spojnice razmake prije.</span><span class="sxs-lookup"><span data-stu-id="83293-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="83293-107">***how-to-Omogući-sudskih procesa-drži***.</span><span class="sxs-lookup"><span data-stu-id="83293-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="83293-108">ID pravila ili bucket ID iz [alkemiji partnera portala](https://alchemyportal.azurewebsites.net) uključiti u polje ms.custom.</span><span class="sxs-lookup"><span data-stu-id="83293-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="83293-109">Franko.</span><span class="sxs-lookup"><span data-stu-id="83293-109">ex.</span></span> <span data-ttu-id="83293-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="83293-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="83293-111">Koristite ostatak metapodatke na vrhu ovu datoteku kao predložak.</span><span class="sxs-lookup"><span data-stu-id="83293-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="83293-112">U [alkemiji partnera portal](https://alchemyportal.azurewebsites.net)pronađite odjeljak **Naslov uvid kupca:** i korištenje koji kao početni pokažite za H1 naslov na uvid.</span><span class="sxs-lookup"><span data-stu-id="83293-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="83293-113">Alkemiji uvide mora imati samo jednu H1 na vrhu ili će prekinuti u proizvodnji.</span><span class="sxs-lookup"><span data-stu-id="83293-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="83293-114">H2s ne renderirati tako koristi **Podebljano** ili druge konvencije za naznaku zasebnim sekcijama.</span><span class="sxs-lookup"><span data-stu-id="83293-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="83293-115">Dalje, ispunite tijelo teksta pomoću materijala skice u sekciji kupca uvide pravilo alkemiji stranice</span><span class="sxs-lookup"><span data-stu-id="83293-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="83293-116">Popisi s grafičkim oznakama su precizno</span><span class="sxs-lookup"><span data-stu-id="83293-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="83293-117">Previše numeriranih popisa</span><span class="sxs-lookup"><span data-stu-id="83293-117">Numbered lists too</span></span>
    1. <span data-ttu-id="83293-118">**Podebljano** i *kurziv* su a-ok</span><span class="sxs-lookup"><span data-stu-id="83293-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="83293-119">Veze uvijek mora biti ili **"veze web" / vanjski** ili **dublje veze elemenata korisničkog Sučelja**, ne i interne veze.</span><span class="sxs-lookup"><span data-stu-id="83293-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="83293-120">Slike su službeno nije podržana u ovom trenutku, ali ga je u roadmap.</span><span class="sxs-lookup"><span data-stu-id="83293-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="83293-121">I to je zaista već je malo predugačak.</span><span class="sxs-lookup"><span data-stu-id="83293-121">And this is really already a bit too long.</span></span> <span data-ttu-id="83293-122">Najbolje je o 400 znakova---</span><span class="sxs-lookup"><span data-stu-id="83293-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="83293-123">Kada vaš sadržaj bude spremna, istaknuti ga uživo granu.</span><span class="sxs-lookup"><span data-stu-id="83293-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="83293-124">Zatim idite na [portal alkemiji partnera](https://alchemyportal.azurewebsites.net) i unesite naziv datoteke u polje url.</span><span class="sxs-lookup"><span data-stu-id="83293-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="83293-125">M</span><span class="sxs-lookup"><span data-stu-id="83293-125">M</span></span>