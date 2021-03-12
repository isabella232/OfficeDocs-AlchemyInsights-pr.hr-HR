---
title: Problemi s API-jem u programu Microsoft Graph
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713472"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="51232-102">Problemi s API-jem u programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51232-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="51232-103">Ova se tema može primijeniti i na programere koji se i dalje koriste API-jem Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="51232-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="51232-104">Međutim **, preporuča se** da koristite Microsoft Graph za sve vaše mape, identitete i upravljanje pristupom.</span><span class="sxs-lookup"><span data-stu-id="51232-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="51232-105">**Problemi s autentifikaciju i autorizacija**</span><span class="sxs-lookup"><span data-stu-id="51232-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="51232-106">Ako aplikacija **ne može nabaviti tokene** za pozivanje programa Microsoft Graph, odaberite **problem s mogućnošću dobivanja tokena programa Access (provjera autentičnosti)** u kategoriji Microsoft Graph da biste dobili konkretniju pomoć i podršku u ovoj temi.</span><span class="sxs-lookup"><span data-stu-id="51232-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="51232-107">Ako aplikacija **dobiva 401 ili 403 pogreške** prilikom pozivanja programa Microsoft Graph, odaberite kategoriju **Dohvaćanje pogreške (autorizacija)** sustava Microsoft Graph API da biste dobili konkretniju pomoć i podršku u ovoj temi.</span><span class="sxs-lookup"><span data-stu-id="51232-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="51232-108">**Želim koristiti Microsoft Graph, ali ne znam gdje početi**</span><span class="sxs-lookup"><span data-stu-id="51232-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="51232-109">Pregled programa Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51232-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="51232-110">Pregled identiteta i upravljanja pristupom u programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51232-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="51232-111">Početak izgradnje aplikacija Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51232-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="51232-112">**Eksplorer za Microsoft Graph** – testiranje programa Microsoft Graph u klijentu ili demo klijentu</span><span class="sxs-lookup"><span data-stu-id="51232-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="51232-113">**Želim koristiti Microsoft Graph, ali podržava li API-ju direktorija v 1.0 koji mi je potreban?**</span><span class="sxs-lookup"><span data-stu-id="51232-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="51232-114">Microsoft Graph Preporučeni je API za upravljanje direktoriju, Identity i Access.</span><span class="sxs-lookup"><span data-stu-id="51232-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="51232-115">No još ima nekoliko praznina između mogućnosti u programu Azure AD Graph i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="51232-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="51232-116">Pregledajte sljedeće članke, što naglašava najnovije razlike koje će vam pomoći u odabiru:</span><span class="sxs-lookup"><span data-stu-id="51232-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="51232-117">Razlike u vrsti resursa između Azure AD Graph i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51232-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="51232-118">Razlike u svojstvima između Azure AD Graph i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51232-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="51232-119">Metode razlike između servisa Azure AD i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51232-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="51232-120">**API koji pozivam ne funkcionira – gdje se mogu dodatno testirati?**</span><span class="sxs-lookup"><span data-stu-id="51232-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="51232-121">**Eksplorer za Microsoft Graph** -Testirajte Microsoft Graph Apis u klijentu ili demo klijentu, a pogledajte i **ogledne upite** u programu Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="51232-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="51232-122">**Moja aplikacija je prespora, a dobiva se i grlo. Koja poboljšanja mogu unijeti?**</span><span class="sxs-lookup"><span data-stu-id="51232-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="51232-123">Ovisno o scenariju, na raspolaganju su vam razne mogućnosti da bi vaša aplikacija bila više performant, a u nekim slučajevima i manje skloni tome da ga servis upravlja (kada ste učinili previše poziva).</span><span class="sxs-lookup"><span data-stu-id="51232-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="51232-124">Najbolja praksa u programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51232-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="51232-125">Zahtjevi za bating</span><span class="sxs-lookup"><span data-stu-id="51232-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="51232-126">Evidentiranje promjena putem Delta upita</span><span class="sxs-lookup"><span data-stu-id="51232-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="51232-127">Primanje obavijesti o promjenama putem webkuke</span><span class="sxs-lookup"><span data-stu-id="51232-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="51232-128">Smjernice za ograničavanje</span><span class="sxs-lookup"><span data-stu-id="51232-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="51232-129">**Gdje mogu pronaći dodatne informacije o pogreškama i poznatim problemima?**</span><span class="sxs-lookup"><span data-stu-id="51232-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="51232-130">Podaci o pogrešci odgovora na Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51232-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="51232-131">Poznati problemi s programom Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51232-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="51232-132">**Gdje mogu provjeriti status dostupnosti i povezivanja servisa?**</span><span class="sxs-lookup"><span data-stu-id="51232-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="51232-133">Dostupnost servisa i povezivanje osnovnih servisa kojima se može pristupiti putem programa Microsoft Graph može utjecati na ukupnu dostupnost i performanse programa Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="51232-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="51232-134">Da biste provjerili stanje servisa Azure Active Directory, provjerite status **sigurnosnih + identifikacijskih** servisa navedenih na [stranici statusa Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="51232-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="51232-135">Za servise sustava Office koji pridonose programu Microsoft Graph provjerite status servisa navedenih na [nadzornoj ploči zdravstvene službe sustava Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="51232-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="51232-136">Pogreške autorizacije u programu Microsoft Graph mogu biti rezultat nekoliko različitih problema, od kojih većina generira pogrešku 401 ili 403.</span><span class="sxs-lookup"><span data-stu-id="51232-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="51232-137">Na primjer, sljedeće može dovesti do pogrešaka autorizacije:</span><span class="sxs-lookup"><span data-stu-id="51232-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="51232-138">Netočni [tijekovi prikupljanja pristupnog tokena](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="51232-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="51232-139">Loše konfigurirani [opsezi dopuštenja](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="51232-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="51232-140">Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="51232-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="51232-141">\**_Kraj podrške za Azure Active Directory Authentication Library (ADAL) i Azure AD Graph API (AAD Graph)_* _</span><span class="sxs-lookup"><span data-stu-id="51232-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="51232-142">_ \* Počevši od 30 Lipanj, 2020 \* \*, više nećemo dodavati nove značajke u ADAL i Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="51232-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="51232-143">I dalje ćemo pružati tehničku podršku i sigurnosna ažuriranja, ali više nećemo pružati ažuriranja značajki.</span><span class="sxs-lookup"><span data-stu-id="51232-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="51232-144">**Počevši od 30 lipnja 2022**, završit ćemo podršku za Adal i Azure ad Graph i više neće pružati tehničku podršku ni Sigurnosno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="51232-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="51232-145">Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće *dobiti nikakvu tehničku podršku ni Sigurnosno ažuriranje*.</span><span class="sxs-lookup"><span data-stu-id="51232-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="51232-146">Aplikacije koje koriste Azure AD Graph nakon tog vremena možda više neće primati odgovore iz krajnjih točaka Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="51232-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="51232-147">**ADAL migracija**</span><span class="sxs-lookup"><span data-stu-id="51232-147">**ADAL Migration**</span></span>

<span data-ttu-id="51232-148">Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) koja ima najnovije značajke i sigurnosna ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="51232-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="51232-149">Ako koristite Microsoftove aplikacije, znajte da je Microsoft u postupku migracije svojih aplikacija u MSAL uz krajnji rok za potporu, čime će se osigurati da koristi MSAL-ove trajne sigurnosti i poboljšanja značajki.</span><span class="sxs-lookup"><span data-stu-id="51232-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="51232-150">Pročitajte najčešća pitanja vezana za ADAL</span><span class="sxs-lookup"><span data-stu-id="51232-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="51232-151">Saznajte kako migrirati aplikacije na platformu</span><span class="sxs-lookup"><span data-stu-id="51232-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="51232-152">Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL, preporučujemo vam da pregledate sve izvorne šifre aplikacija i ako je primjenjivo, obratite se svim pružateljima programa ISVs ili aplikacije.</span><span class="sxs-lookup"><span data-stu-id="51232-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="51232-153">Microsoftova podrška također vam može pružiti popis svih aplikacija koje nisu Microsoftove ADAL u vašem klijentu.</span><span class="sxs-lookup"><span data-stu-id="51232-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="51232-154">**Migracija grafikona AAD**</span><span class="sxs-lookup"><span data-stu-id="51232-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="51232-155">Za aplikacije koje koriste Azure AD Graph, slijedite upute da biste [migrirali aplikacije Azure ad Graph u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="51232-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="51232-156">[Naš popis za migraciju pruža točku početka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="51232-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="51232-157">Vaš portal za registraciju Azure aplikacija prikazuje koje aplikacije koriste AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="51232-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="51232-158">Preporučujemo da pregledate izvorni kod svih aplikacija i ako je primjenjivo obratite se svim ISV-ovima ili davateljima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="51232-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="51232-159">Microsoftova podrška može vam pružiti i popis svih korištenja AAD grafikona u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="51232-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="51232-160">Da bi aplikacija pristupio podacima u programu Microsoft Graph, korisnik ili administrator mora mu dodijeliti ispravne dozvole putem postupka pristanka.</span><span class="sxs-lookup"><span data-stu-id="51232-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="51232-161">[Referenca dozvola za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) prikazuje popise dozvola povezanih sa svakim glavnim skupom programa Microsoft Graph Apis.</span><span class="sxs-lookup"><span data-stu-id="51232-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="51232-162">Nudi i upute za korištenje dozvola.</span><span class="sxs-lookup"><span data-stu-id="51232-162">It also provides guidance about how to use the permissions.</span></span>
