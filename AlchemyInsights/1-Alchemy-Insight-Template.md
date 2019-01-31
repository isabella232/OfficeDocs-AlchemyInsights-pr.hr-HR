---
title: 'isti kao naziv datoteke je najbolje [pravilo #-opis]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662922"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="3f205-102">Potreban klijent nasuprotne H1, H2 ne radi</span><span class="sxs-lookup"><span data-stu-id="3f205-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="3f205-103">Primjer teksta Blokiraj - slijedite ove upute:</span><span class="sxs-lookup"><span data-stu-id="3f205-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="3f205-104">Datoteke u mapi **AlchemyInsights** treba imati pravilo ID i naziv pravila s [portala alkemiji partnera](https://alchemyportal.azurewebsites.net) u naziv datoteke.</span><span class="sxs-lookup"><span data-stu-id="3f205-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="3f205-p101">Ex. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="3f205-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="3f205-p102">Koristite metapodatke na vrhu ovu datoteku kao predložak. Ništa drugo nije potrebna.</span><span class="sxs-lookup"><span data-stu-id="3f205-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="3f205-109">U [alkemiji partnera portal](https://alchemyportal.azurewebsites.net)pronađite odjeljak **Naslov uvid kupca:** i korištenje koji kao početni pokažite za H1 naslov na uvid.</span><span class="sxs-lookup"><span data-stu-id="3f205-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="3f205-p103">Alkemiji uvide mora imati samo jednu H1 na vrhu ili će prekinuti u proizvodnji. H2s ne renderirati tako koristi **Podebljano** ili druge konvencije za naznaku zasebnim sekcijama.</span><span class="sxs-lookup"><span data-stu-id="3f205-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="3f205-112">Dalje, ispunite tijelo teksta pomoću materijala skice u sekciji kupca uvide pravilo alkemiji stranice</span><span class="sxs-lookup"><span data-stu-id="3f205-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="3f205-113">Popisi s grafičkim oznakama su precizno</span><span class="sxs-lookup"><span data-stu-id="3f205-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="3f205-114">Previše numeriranih popisa</span><span class="sxs-lookup"><span data-stu-id="3f205-114">Numbered lists too</span></span>
    1. <span data-ttu-id="3f205-115">**Podebljano** i *kurziv* su a-ok</span><span class="sxs-lookup"><span data-stu-id="3f205-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="3f205-116">Veze uvijek mora biti ili **"veze web" / vanjski** ili **dublje veze elemenata korisničkog Sučelja**, ne i interne veze.</span><span class="sxs-lookup"><span data-stu-id="3f205-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="3f205-p104">I to je zaista već je malo predugačak. Najbolje je o 400 znakova---</span><span class="sxs-lookup"><span data-stu-id="3f205-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="3f205-p105">Kada vaš sadržaj bude spremna, istaknuti ga uživo granu. Zatim idite na [portal alkemiji partnera](https://alchemyportal.azurewebsites.net) i unesite naziv datoteke u polje url. Provjerite uvid pregledavaju i objavljuju kaže "da", a zatim kliknite pravilo ažuriranja. (To će izgledati prettier u novu verziju portala - otpustite uskoro.)</span><span class="sxs-lookup"><span data-stu-id="3f205-p105">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. (This will look prettier in the new version of the portal - releasing soon.)</span></span>

![URL polje](media/for-content-team.PNG)

