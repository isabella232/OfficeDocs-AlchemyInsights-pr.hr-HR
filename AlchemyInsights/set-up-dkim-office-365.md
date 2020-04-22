---
title: Postavljanje DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645664"
---
# <a name="setup-dkim"></a><span data-ttu-id="e653a-102">Postavljanje DKIM</span><span class="sxs-lookup"><span data-stu-id="e653a-102">Setup DKIM</span></span>

<span data-ttu-id="e653a-103">Potpune upute za konfiguriranje DKIM-a za prilagođene domene u sustavu Microsoft 365 [su ovdje](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="e653a-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="e653a-104">Za **svaku** prilagođenu domenu morate stvoriti **dva** DKIM CNAME zapisa na servisu za hostiranje DNS-a vaše domene (obično registraru domene).</span><span class="sxs-lookup"><span data-stu-id="e653a-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="e653a-105">Na primjer, contoso.com i fourthcoffee.com zahtijevaju četiri DKIM CNAME zapisa: dva za contoso.com i dva za fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="e653a-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="e653a-106">DKIM CNAME zapisi za **svaku** prilagođenu domenu koriste sljedeće oblike:</span><span class="sxs-lookup"><span data-stu-id="e653a-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="e653a-107">**Ime glavnog računala**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="e653a-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="e653a-108">**Točke na adresu ili vrijednost:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="e653a-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="e653a-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="e653a-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="e653a-110">**Ime glavnog računala**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="e653a-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="e653a-111">**Točke na adresu ili vrijednost:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="e653a-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="e653a-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="e653a-112">**TTL**: 3600</span></span>

   <span data-ttu-id="e653a-113">\<DomainGUID\> je tekst s `.mail.protection.outlook.com` lijeve strane u prilagođenom MX zapisu `contoso-com` za prilagođenu domenu (na primjer, za contoso.com domene).</span><span class="sxs-lookup"><span data-stu-id="e653a-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="e653a-114">\<InitialDomain\> je domena koju ste koristili kada ste se prijavili za Microsoft 365 (na primjer, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="e653a-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="e653a-115">Nakon što stvorite CNAME zapise za prilagođene domene, izvršite sljedeće upute:</span><span class="sxs-lookup"><span data-stu-id="e653a-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="e653a-116">A.</span><span class="sxs-lookup"><span data-stu-id="e653a-116">a.</span></span> <span data-ttu-id="e653a-117">[prijavite se u Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomoću računa tvrtke ili obrazovne ustanove.</span><span class="sxs-lookup"><span data-stu-id="e653a-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="e653a-118">B.</span><span class="sxs-lookup"><span data-stu-id="e653a-118">b.</span></span> <span data-ttu-id="e653a-119">Odaberite ikonu pokretača aplikacija u gornjem lijevom kutu i odaberite **Administrator**.</span><span class="sxs-lookup"><span data-stu-id="e653a-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="e653a-120">C.</span><span class="sxs-lookup"><span data-stu-id="e653a-120">c.</span></span> <span data-ttu-id="e653a-121">U navigaciji u donjem lijevom kutu **proširite Administrator** i odaberite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="e653a-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="e653a-122">D.</span><span class="sxs-lookup"><span data-stu-id="e653a-122">d.</span></span> <span data-ttu-id="e653a-123">Idite na **Zaštita** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="e653a-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="e653a-124">E.</span><span class="sxs-lookup"><span data-stu-id="e653a-124">e.</span></span> <span data-ttu-id="e653a-125">Odaberite domenu , a zatim odaberite **Omogući** za **potpisivanje poruka za ovu domenu s DKIM potpisima**.</span><span class="sxs-lookup"><span data-stu-id="e653a-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="e653a-126">Ponovite ovaj korak za svaku prilagođenu domenu.</span><span class="sxs-lookup"><span data-stu-id="e653a-126">Repeat this step for each custom domain.</span></span>
