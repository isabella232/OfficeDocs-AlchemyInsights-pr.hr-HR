---
title: Postavljanje DKIM u sustavu Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764923"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="533e9-102">Postavljanje DKIM u sustavu Office 365</span><span class="sxs-lookup"><span data-stu-id="533e9-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="533e9-103">Dovršeno upute za konfiguriranje DKIM za prilagođenih domena u sustavu Office 365 su [ovdje](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="533e9-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="533e9-104">Za **svaku** prilagođenu domenu, morate stvoriti **dva** DKIM CNAME zapise na vaše domene DNS pružatelju usluge (obično Registrator domene).</span><span class="sxs-lookup"><span data-stu-id="533e9-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="533e9-105">Ako, na primjer, contoso.com i fourthcoffee.com zahtijevaju četiri zapisa DKIM CNAME: dva za contoso.com i dva za fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="533e9-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="533e9-106">DKIM CNAME zapisa za **svaku** prilagođenu domenu koristite sljedeće formate:</span><span class="sxs-lookup"><span data-stu-id="533e9-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="533e9-107">**Naziv glavnog računala**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="533e9-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="533e9-108">**Točke adresu ili vrijednost**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="533e9-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="533e9-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="533e9-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="533e9-110">**Naziv glavnog računala**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="533e9-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="533e9-111">**Točke adresu ili vrijednost**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="533e9-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="533e9-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="533e9-112">**TTL**: 3600</span></span>

   <span data-ttu-id="533e9-113">\<DomainGUID\> je tekst lijevo od `.mail.protection.outlook.com` u prilagođene MX zapisa za prilagođene domene (na primjer, `contoso-com` za contoso.com domene).</span><span class="sxs-lookup"><span data-stu-id="533e9-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="533e9-114">\<InitialDomain\> je domene koji ste koristili kada ste se prijavili za Office 365 (na primjer, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="533e9-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="533e9-115">Nakon što ste stvorili zapise CNAME za prilagođene domene, dovršite sljedeće upute:</span><span class="sxs-lookup"><span data-stu-id="533e9-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="533e9-116">na.</span><span class="sxs-lookup"><span data-stu-id="533e9-116">a.</span></span> <span data-ttu-id="533e9-117">[Prijavite se u Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) s računom poslu ili u školi.</span><span class="sxs-lookup"><span data-stu-id="533e9-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="533e9-118">b.</span><span class="sxs-lookup"><span data-stu-id="533e9-118">b.</span></span> <span data-ttu-id="533e9-119">Odaberite ikonu pokretača app u gornju lijevu i odaberite **Admin**.</span><span class="sxs-lookup"><span data-stu-id="533e9-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="533e9-120">c.</span><span class="sxs-lookup"><span data-stu-id="533e9-120">c.</span></span> <span data-ttu-id="533e9-121">U donjem lijevom navigacijskom proširite **Admin** i odaberite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="533e9-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="533e9-122">d.</span><span class="sxs-lookup"><span data-stu-id="533e9-122">d.</span></span> <span data-ttu-id="533e9-123">Idi na **zaštitu** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="533e9-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="533e9-124">e.</span><span class="sxs-lookup"><span data-stu-id="533e9-124">e.</span></span> <span data-ttu-id="533e9-125">Odaberite domenu, a zatim odaberite **Omogući** za **potpisivanje poruke za ovu domenu s potpisima DKIM**.</span><span class="sxs-lookup"><span data-stu-id="533e9-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="533e9-126">Ponovite ovaj korak za svaku prilagođenu domenu.</span><span class="sxs-lookup"><span data-stu-id="533e9-126">Repeat this step for each custom domain.</span></span>
