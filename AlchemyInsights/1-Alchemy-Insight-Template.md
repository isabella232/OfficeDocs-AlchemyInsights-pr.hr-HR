---
title: 'isti kao naziv datoteke je najbolje [pravilo #-opis]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634496"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="d18ce-102">Potrebna alkemiji zaglavlje H1, H2's ne rade.</span><span class="sxs-lookup"><span data-stu-id="d18ce-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="d18ce-103">Najbolje prakse i smjernice za autorizaciju alkemiji:</span><span class="sxs-lookup"><span data-stu-id="d18ce-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="d18ce-104">**Ugnijezditi alkemiji uvida u mapama**- će ovo prelomiti strukturu url.</span><span class="sxs-lookup"><span data-stu-id="d18ce-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="d18ce-105">Možemo traženu u popravljanju to.</span><span class="sxs-lookup"><span data-stu-id="d18ce-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="d18ce-106">Datoteke u mapi **AlchemyInsights** treba imati pravilo ID i naziv pravila s [portala alkemiji partnera](https://alchemyportal.azurewebsites.net) u naziv datoteke.</span><span class="sxs-lookup"><span data-stu-id="d18ce-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="d18ce-107">Franko.</span><span class="sxs-lookup"><span data-stu-id="d18ce-107">ex.</span></span> <span data-ttu-id="d18ce-108">***976-How-to-enable-litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="d18ce-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="d18ce-109">Koristite metapodatke na vrhu ovu datoteku kao predložak.</span><span class="sxs-lookup"><span data-stu-id="d18ce-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="d18ce-110">Ništa drugo nije potrebna.</span><span class="sxs-lookup"><span data-stu-id="d18ce-110">Nothing else is required.</span></span>
1. <span data-ttu-id="d18ce-111">U [alkemiji partnera portal](https://alchemyportal.azurewebsites.net)pronađite odjeljak **Naslov uvid kupca:** i korištenje koji kao početni pokažite za H1 naslov na uvid.</span><span class="sxs-lookup"><span data-stu-id="d18ce-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="d18ce-112">Alkemiji uvide mora imati samo jednu H1 na vrhu ili će prekinuti u proizvodnji.</span><span class="sxs-lookup"><span data-stu-id="d18ce-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="d18ce-113">H2s ne renderirati tako koristi **Podebljano** ili druge konvencije za naznaku zasebnim sekcijama.</span><span class="sxs-lookup"><span data-stu-id="d18ce-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="d18ce-114">Dalje, ispunite tijelo teksta pomoću materijala skice u sekciji kupca uvide pravilo alkemiji stranice</span><span class="sxs-lookup"><span data-stu-id="d18ce-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="d18ce-115">Popisi s grafičkim oznakama su precizno</span><span class="sxs-lookup"><span data-stu-id="d18ce-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="d18ce-116">Previše numeriranih popisa</span><span class="sxs-lookup"><span data-stu-id="d18ce-116">Numbered lists too</span></span>
    1. <span data-ttu-id="d18ce-117">**Podebljano** i *kurziv* su a-ok</span><span class="sxs-lookup"><span data-stu-id="d18ce-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="d18ce-118">Veze uvijek mora biti ili **"veze web" / vanjski** ili **dublje veze elemenata korisničkog Sučelja**, ne i interne veze.</span><span class="sxs-lookup"><span data-stu-id="d18ce-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="d18ce-119">I to je zaista već je malo predugačak.</span><span class="sxs-lookup"><span data-stu-id="d18ce-119">And this is really already a bit too long.</span></span> <span data-ttu-id="d18ce-120">Najbolje je o 400 znakova---</span><span class="sxs-lookup"><span data-stu-id="d18ce-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="d18ce-121">Kada vaš sadržaj bude spremna, istaknuti ga uživo granu.</span><span class="sxs-lookup"><span data-stu-id="d18ce-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="d18ce-122">Zatim idite na [portal alkemiji partnera](https://alchemyportal.azurewebsites.net) i unesite naziv datoteke u polje url.</span><span class="sxs-lookup"><span data-stu-id="d18ce-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="d18ce-123">Provjerite uvid pregledavaju i objavljuju kaže "da", a zatim kliknite pravilo ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="d18ce-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="d18ce-124">**(To će izgledati prettier u novu verziju portala - otpustite uskoro.)** 
 ![url polje](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="d18ce-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

