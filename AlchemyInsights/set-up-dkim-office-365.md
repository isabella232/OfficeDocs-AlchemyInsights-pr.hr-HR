---
title: Postavljanje funkcije
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808699"
---
# <a name="setup-dkim"></a><span data-ttu-id="5a8ab-102">Postavljanje funkcije</span><span class="sxs-lookup"><span data-stu-id="5a8ab-102">Setup DKIM</span></span>

<span data-ttu-id="5a8ab-103">U programu Microsoft [365 nalaze se](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)potpune upute za konfiguriranje servisa d ' dekima za prilagođene domene u Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="5a8ab-104">Za **svaku** prilagođenu domenu morate stvoriti **dva** DKIM CNAME zapisa na servisu za hostiranje DNS-a u domeni (obično je registrar domena).</span><span class="sxs-lookup"><span data-stu-id="5a8ab-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="5a8ab-105">Primjerice, contoso.com i fourthcoffee.com zahtijevaju četiri DKIM CNAME zapisa: dva za contoso.com i dva za fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="5a8ab-106">Zapisi u programu defunkcija CNAME za **svaku** prilagođenu domenu koriste sljedeće oblike:</span><span class="sxs-lookup"><span data-stu-id="5a8ab-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="5a8ab-107">**Naziv glavnog računala**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="5a8ab-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="5a8ab-108">**Upućuje na adresu ili vrijednost**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="5a8ab-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="5a8ab-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="5a8ab-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="5a8ab-110">**Naziv glavnog računala**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="5a8ab-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="5a8ab-111">**Upućuje na adresu ili vrijednost**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="5a8ab-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="5a8ab-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="5a8ab-112">**TTL**: 3600</span></span>

   <span data-ttu-id="5a8ab-113">\<DomainGUID\> je li tekst s desne strane `.mail.protection.outlook.com` u PRILAGOĐENOM MX zapisu za prilagođenu domenu (na primjer, `contoso-com` za domenu contoso.com).</span><span class="sxs-lookup"><span data-stu-id="5a8ab-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="5a8ab-114">\<InitialDomain\> domena koju ste koristili kada ste se prijavili za Microsoft 365 (na primjer, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="5a8ab-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="5a8ab-115">Kada stvorite CNAME zapise za prilagođene domene, ispunite sljedeće upute:</span><span class="sxs-lookup"><span data-stu-id="5a8ab-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="5a8ab-116">je.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-116">a.</span></span> <span data-ttu-id="5a8ab-117">[prijavite se u Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomoću računa tvrtke ili obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="5a8ab-118">b.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-118">b.</span></span> <span data-ttu-id="5a8ab-119">U gornjem desnom kutu odaberite ikonu Pokretača aplikacija, a zatim **administrator**.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="5a8ab-120">c.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-120">c.</span></span> <span data-ttu-id="5a8ab-121">U donjem desnom navigacijskom oknu proširite **administrator** i odaberite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="5a8ab-122">d.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-122">d.</span></span> <span data-ttu-id="5a8ab-123">Idite na **zaštitu**  >  **d-kim**.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="5a8ab-124">e.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-124">e.</span></span> <span data-ttu-id="5a8ab-125">Odaberite domenu, a zatim odaberite **Omogući** za **potpisivanje poruka za ovu domenu s DKIM potpisima**.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="5a8ab-126">Ponovite ovaj korak za svaku prilagođenu domenu.</span><span class="sxs-lookup"><span data-stu-id="5a8ab-126">Repeat this step for each custom domain.</span></span>
