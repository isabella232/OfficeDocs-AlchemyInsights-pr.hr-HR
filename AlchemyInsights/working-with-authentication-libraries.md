---
title: Rad s bibliotekama za provjeru autentičnosti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035016"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="830ae-102">Rad s bibliotekama za provjeru autentičnosti</span><span class="sxs-lookup"><span data-stu-id="830ae-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="830ae-103">Da biste riješili problem biblioteke programa Microsoft Authentication (MSAL), učinite sljedeće preporučene korake:</span><span class="sxs-lookup"><span data-stu-id="830ae-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="830ae-104">**Rad sa programom MSAL**: [biblioteke za provjeru autentičnosti Microsoftove platforme identiteta](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – u ovom se članku sadrži Podrška za biblioteku Microsoft Authentication za nekoliko vrsta aplikacija.</span><span class="sxs-lookup"><span data-stu-id="830ae-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="830ae-105">Sadrži veze na izvorni kod biblioteke. Gdje nabaviti paket za projekt aplikacije? i podržava li biblioteka korisničke prijave (provjera autentičnosti), pristup zaštićenim web-API-Jima (autorizacija) ili oboje.</span><span class="sxs-lookup"><span data-stu-id="830ae-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="830ae-106">**Otklanjanje poteškoća s provjerom autentičnosti**: msal podržava nekoliko tokova provjere autentičnosti za korištenje u različitim scenarijima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="830ae-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="830ae-107">Ovisno o tome kako je vaša klijentska aplikacija izgrađena, MSAL može koristiti jedan ili više tokova provjere autentičnosti koje podržava Microsoftova platforma identiteta.</span><span class="sxs-lookup"><span data-stu-id="830ae-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="830ae-108">Ovi tijekovi mogu proizvesti nekoliko vrsta tokena i autorizacije, te zahtijevati različite tokene da bi funkcionisali.</span><span class="sxs-lookup"><span data-stu-id="830ae-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="830ae-109">**Token za Access**: [tokeni za pristup Microsoftovoj platformi za identitete](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -Naučite kako API može provjeriti valjanost i koristiti zahtjeve u pristupnom toknu.</span><span class="sxs-lookup"><span data-stu-id="830ae-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="830ae-110">Sva dokumentacija u ovom članku, osim ako je navedeno, primjenjuje se samo na tokene izdane za API-je koje ste registrirali.</span><span class="sxs-lookup"><span data-stu-id="830ae-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="830ae-111">Ne primjenjuje se na tokene izdane za API-je u vlasništvu Microsofta, niti se ti tokeni mogu koristiti za provjeru načina na koji će Microsoftova platforma za identitete izdati žetone za neki API koji ste stvorili.</span><span class="sxs-lookup"><span data-stu-id="830ae-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="830ae-112">**Kraj podrške za biblioteku autentičnosti servisa Azure Active Directory (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="830ae-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="830ae-113">**Počevši od 30 lipnja 2020,** više nećemo dodavati nove značajke u AD Graph Adal i Azure.</span><span class="sxs-lookup"><span data-stu-id="830ae-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="830ae-114">I dalje ćemo pružati tehničku podršku i sigurnosna ažuriranja, ali više nećemo pružati ažuriranja značajki.</span><span class="sxs-lookup"><span data-stu-id="830ae-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="830ae-115">**Počevši od 30 lipnja 2022,** završit ćemo podršku za Adal i Azure ad Graph i više neće pružati tehničku podršku ni Sigurnosno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="830ae-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="830ae-116">Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće *dobiti nikakvu tehničku podršku ni Sigurnosno ažuriranje*.</span><span class="sxs-lookup"><span data-stu-id="830ae-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="830ae-117">Aplikacije koje koriste Azure AD Graph nakon tog vremena možda više neće primati odgovore iz krajnjih točaka Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="830ae-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="830ae-118">**ADAL migracija**</span><span class="sxs-lookup"><span data-stu-id="830ae-118">**ADAL Migration**</span></span>

- <span data-ttu-id="830ae-119">Preporučujemo ažuriranje MSAL-a, koji sadrži najnovije značajke i sigurnosno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="830ae-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="830ae-120">Ako koristite Microsoftove aplikacije, znajte da je Microsoft u postupku migracije svojih aplikacija u MSAL uz krajnji rok podrške za MSAL, čime će se osigurati da će imati koristi u trajnoj sigurnosti i poboljšanjima značajki koje je mala.</span><span class="sxs-lookup"><span data-stu-id="830ae-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="830ae-121">[Pročitajte najčešća pitanja o dodatku](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="830ae-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="830ae-122">[Saznajte kako migrirati aplikacije na osnovi po platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="830ae-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="830ae-123">Ako nakon čitanja vodiča za platformu aplikacije imate dodatna pitanja, možete objavljivati na servisu [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) pomoću oznake [Azure-ad-Adal-depretcation] ili otvoriti problem u spremištu za GitHub biblioteke.</span><span class="sxs-lookup"><span data-stu-id="830ae-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="830ae-124">Pogledajte odjeljak [Jezici i okviri](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) u članku **Pregled msal** -a za veze na repo svake biblioteke.</span><span class="sxs-lookup"><span data-stu-id="830ae-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="830ae-125">**Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL**, preporučujemo da pregledate izvorni kod svih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="830ae-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="830ae-126">Ako je primjenjivo, obratite se svim neovisnim dobavljačima softvera (ISVs) ili pružateljima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="830ae-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="830ae-127">Microsoftova podrška također vam može pružiti popis svih aplikacija koje nisu Microsoftove ADAL u vašem klijentu.</span><span class="sxs-lookup"><span data-stu-id="830ae-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







