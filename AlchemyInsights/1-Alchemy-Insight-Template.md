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
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697122"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="4eb33-102">Potrebna alkemiji zaglavlje H1, H2's ne rade.</span><span class="sxs-lookup"><span data-stu-id="4eb33-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="4eb33-103">Najbolje prakse i smjernice za autorizaciju alkemiji:</span><span class="sxs-lookup"><span data-stu-id="4eb33-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="4eb33-p101">**Ugnijezditi alkemiji uvida u mapama**- će ovo prelomiti strukturu url. Možemo traženu u popravljanju to.</span><span class="sxs-lookup"><span data-stu-id="4eb33-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="4eb33-106">Datoteke u mapi **AlchemyInsights** treba imati pravilo ID i naziv pravila s [portala alkemiji partnera](https://alchemyportal.azurewebsites.net) u naziv datoteke.</span><span class="sxs-lookup"><span data-stu-id="4eb33-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="4eb33-p102">Ex. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="4eb33-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="4eb33-p103">Koristite metapodatke na vrhu ovu datoteku kao predložak. Ništa drugo nije potrebna.</span><span class="sxs-lookup"><span data-stu-id="4eb33-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="4eb33-111">U [alkemiji partnera portal](https://alchemyportal.azurewebsites.net)pronađite odjeljak **Naslov uvid kupca:** i korištenje koji kao početni pokažite za H1 naslov na uvid.</span><span class="sxs-lookup"><span data-stu-id="4eb33-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="4eb33-p104">Alkemiji uvide mora imati samo jednu H1 na vrhu ili će prekinuti u proizvodnji. H2s ne renderirati tako koristi **Podebljano** ili druge konvencije za naznaku zasebnim sekcijama.</span><span class="sxs-lookup"><span data-stu-id="4eb33-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="4eb33-114">Dalje, ispunite tijelo teksta pomoću materijala skice u sekciji kupca uvide pravilo alkemiji stranice</span><span class="sxs-lookup"><span data-stu-id="4eb33-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="4eb33-115">Popisi s grafičkim oznakama su precizno</span><span class="sxs-lookup"><span data-stu-id="4eb33-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="4eb33-116">Previše numeriranih popisa</span><span class="sxs-lookup"><span data-stu-id="4eb33-116">Numbered lists too</span></span>
    1. <span data-ttu-id="4eb33-117">**Podebljano** i *kurziv* su a-ok</span><span class="sxs-lookup"><span data-stu-id="4eb33-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="4eb33-118">Veze uvijek mora biti ili **"veze web" / vanjski** ili **dublje veze elemenata korisničkog Sučelja**, ne i interne veze.</span><span class="sxs-lookup"><span data-stu-id="4eb33-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="4eb33-p105">I to je zaista već je malo predugačak. Najbolje je o 400 znakova---</span><span class="sxs-lookup"><span data-stu-id="4eb33-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="4eb33-p106">Kada vaš sadržaj bude spremna, istaknuti ga uživo granu. Zatim idite na [portal alkemiji partnera](https://alchemyportal.azurewebsites.net) i unesite naziv datoteke u polje url. Provjerite uvid pregledavaju i objavljuju kaže "da", a zatim kliknite pravilo ažuriranja. **(To će izgledati prettier u novu verziju portala - otpustite uskoro.)** 
 ![url polje](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="4eb33-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

