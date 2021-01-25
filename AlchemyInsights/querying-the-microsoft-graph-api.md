---
title: Postavljanje upita u API-ju programa Microsoft Graph
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974215"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="78090-102">Postavljanje upita u API-ju programa Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="78090-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="78090-103">Ova se tema može primijeniti i na programere koji se i dalje koriste API-jem Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="78090-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="78090-104">Međutim **, preporuča se** da koristite Microsoft Graph za sve vaše mape, identitete i upravljanje pristupom.</span><span class="sxs-lookup"><span data-stu-id="78090-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="78090-105">**Problemi s autentifikaciju i autorizacija**</span><span class="sxs-lookup"><span data-stu-id="78090-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="78090-106">Ako aplikacija **ne može nabaviti tokene** za pozivanje programa Microsoft Graph, odaberite **problem s mogućnošću dobivanja tokena programa Access (provjera autentičnosti)** u kategoriji Microsoft Graph da biste dobili konkretniju pomoć i podršku u ovoj temi.</span><span class="sxs-lookup"><span data-stu-id="78090-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="78090-107">Ako aplikacija **dobiva 401 ili 403 pogreške** prilikom pozivanja programa Microsoft Graph, odaberite kategoriju **Dohvaćanje pogreške (autorizacija)** sustava Microsoft Graph API da biste dobili konkretniju pomoć i podršku u ovoj temi.</span><span class="sxs-lookup"><span data-stu-id="78090-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="78090-108">**Želim koristiti Microsoft Graph, ali ne znam gdje početi**</span><span class="sxs-lookup"><span data-stu-id="78090-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="78090-109">Dodatne informacije o programu Microsoft Graph potražite u člancima:</span><span class="sxs-lookup"><span data-stu-id="78090-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="78090-110">Pregled programa Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="78090-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="78090-111">Pregled identiteta i upravljanja pristupom u programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="78090-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="78090-112">Početak izgradnje aplikacija Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="78090-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="78090-113">**Eksplorer za Microsoft Graph** – testiranje programa Microsoft Graph u klijentu ili demo klijentu</span><span class="sxs-lookup"><span data-stu-id="78090-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="78090-114">**Želim koristiti Microsoft Graph, ali podržava li API-ju direktorija v 1.0 koji mi je potreban?**</span><span class="sxs-lookup"><span data-stu-id="78090-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="78090-115">Microsoft Graph Preporučeni je API za upravljanje direktoriju, Identity i Access.</span><span class="sxs-lookup"><span data-stu-id="78090-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="78090-116">No još ima nekoliko praznina između mogućnosti u programu Azure AD Graph i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="78090-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="78090-117">Pregledajte sljedeće članke, što naglašava najnovije razlike koje će vam pomoći u odabiru:</span><span class="sxs-lookup"><span data-stu-id="78090-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="78090-118">Razlike u vrsti resursa između Azure AD Graph i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="78090-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="78090-119">Razlike u svojstvima između Azure AD Graph i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="78090-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="78090-120">Metode razlike između servisa Azure AD i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="78090-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="78090-121">**Kada upitam *korisnički* objekt, nedostaju mnoga njegova svojstva**</span><span class="sxs-lookup"><span data-stu-id="78090-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="78090-122">`GET https://graph.microsoft.com/v1.0/users` vraća samo 11 svojstava, jer Microsoft Graph automatski odabire zadani skup *korisničkih* svojstava za povratak.</span><span class="sxs-lookup"><span data-stu-id="78090-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="78090-123">Ako vam je potrebna druga *korisnička* svojstva, koristite $Select da biste odabrali svojstva koja je potrebna aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="78090-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="78090-124">Najprije isprobajte u programu **Microsoft Graph Explorer** .</span><span class="sxs-lookup"><span data-stu-id="78090-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="78090-125">**Neke su vrijednosti korisničkog svojstva *Null* iako znam da su postavljeni**</span><span class="sxs-lookup"><span data-stu-id="78090-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="78090-126">Najvjerojatnije je objašnjenje da je aplikaciji dodijeljen *korisnik. ReadBasic. sve* dozvole.</span><span class="sxs-lookup"><span data-stu-id="78090-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="78090-127">Time se aplikaciji omogućuje čitanje ograničenog skupa korisničkih svojstava, vraćanje svih ostalih svojstava kao null, čak i ako su prethodno bili postavljeni.</span><span class="sxs-lookup"><span data-stu-id="78090-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="78090-128">Pokušajte dodijelite korisniku aplikacije *. pročitajte. svi* dozvola umjesto.</span><span class="sxs-lookup"><span data-stu-id="78090-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="78090-129">Dodatne informacije potražite u [članku korisničke dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="78090-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="78090-130">**Imam problema s upotrebom parametara OData Query za filtriranje podataka u mojim zahtjevima**</span><span class="sxs-lookup"><span data-stu-id="78090-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="78090-131">Dok Microsoft Graph podržava širok raspon parametara OData upita, mnogi od tih parametara nisu u potpunosti podržani od strane imeničkih servisa (resursa koji nasljeđuju od *Directoryobject*) u programu Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="78090-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="78090-132">Ista ograničenja koja su bila prisutna u programu Azure AD Graph najviše su dio u programu Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="78090-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="78090-133">**Nije podržano**: $count, $search i $filter na *Null* ili *Not null* vrijednosti</span><span class="sxs-lookup"><span data-stu-id="78090-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="78090-134">**Nije podržano**: $filter na određenim svojstvima (Pogledajte teme resursa na kojima je moguće filtrirati svojstva)</span><span class="sxs-lookup"><span data-stu-id="78090-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="78090-135">**Nije podržano**: straničenje, filtriranje i sortiranje u isto vrijeme</span><span class="sxs-lookup"><span data-stu-id="78090-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="78090-136">**Nije podržano**: filtriranje odnosa.</span><span class="sxs-lookup"><span data-stu-id="78090-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="78090-137">Na primjer – Pronađite sve članove grupe za inženjerstvo u Velikoj Britaniji.</span><span class="sxs-lookup"><span data-stu-id="78090-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="78090-138">**Djelomična podrška**: $OrderBy na *korisniku* (samo DisplayName i UserPrincipalName) i *grupa*</span><span class="sxs-lookup"><span data-stu-id="78090-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="78090-139">**Djelomična podrška**: $filter (podržava samo *IQ*, *Startswith*, *or*, *and* i ograničenu *bilo koju*) podršku, $Expand (proširenje odnosa jednog objekta vraća sve odnose, ali je ograničena zbirka odnosa objekata)</span><span class="sxs-lookup"><span data-stu-id="78090-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="78090-140">Dodatne informacije potražite u članku [Prilagodba odgovora s parametrima upita](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="78090-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="78090-141">**API koji pozivam ne funkcionira – gdje mogu učiniti više testiranja?**</span><span class="sxs-lookup"><span data-stu-id="78090-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="78090-142">**Eksplorer za Microsoft Graph** -Testirajte Microsoft Graph Apis u klijentu ili demo klijentu, a pogledajte i **ogledne upite** u programu Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="78090-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="78090-143">**Prilikom upita za podatke čini se kao da dobivam nepotpun skup podataka natrag**</span><span class="sxs-lookup"><span data-stu-id="78090-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="78090-144">Ako postavljate upit za zbirku (kao što su *korisnici*), Microsoft Graph koristi ograničenja stranice poslužitelja pa se rezultati uvijek vraćaju s zadanom veličinom stranice.</span><span class="sxs-lookup"><span data-stu-id="78090-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="78090-145">Aplikacija bi uvijek trebala očekivati da će se na nju prikazivati zbirke vraćene iz servisa.</span><span class="sxs-lookup"><span data-stu-id="78090-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="78090-146">Dodatne informacije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="78090-146">For more information, see:</span></span>

- [<span data-ttu-id="78090-147">Najbolja praksa u programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="78090-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="78090-148">Podaci o programu Microsoft Graph u aplikaciji</span><span class="sxs-lookup"><span data-stu-id="78090-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="78090-149">**Moja aplikacija je prespora, a dobiva se i grlo. Koja poboljšanja mogu unijeti?**</span><span class="sxs-lookup"><span data-stu-id="78090-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="78090-150">Ovisno o scenariju, na raspolaganju su vam razne mogućnosti da bi vam aplikacija bila više performant, a u nekim slučajevima i manje sklona tome da vas servis upravlja (kada stvarate previše poziva).</span><span class="sxs-lookup"><span data-stu-id="78090-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="78090-151">Dodatne informacije potražite u člancima:</span><span class="sxs-lookup"><span data-stu-id="78090-151">To learn more, see:</span></span>

- [<span data-ttu-id="78090-152">Najbolja praksa u programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="78090-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="78090-153">Zahtjevi za bating</span><span class="sxs-lookup"><span data-stu-id="78090-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="78090-154">Evidentiranje promjena putem Delta upita</span><span class="sxs-lookup"><span data-stu-id="78090-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="78090-155">Primanje obavijesti o promjenama putem webkuke</span><span class="sxs-lookup"><span data-stu-id="78090-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="78090-156">Smjernice za ograničavanje</span><span class="sxs-lookup"><span data-stu-id="78090-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="78090-157">**Gdje mogu pronaći dodatne informacije o pogreškama i poznatim problemima?**</span><span class="sxs-lookup"><span data-stu-id="78090-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="78090-158">Podaci o pogrešci odgovora na Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="78090-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="78090-159">Poznati problemi s programom Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="78090-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="78090-160">**Gdje mogu provjeriti status dostupnosti i povezivanja servisa?**</span><span class="sxs-lookup"><span data-stu-id="78090-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="78090-161">Dostupnost servisa i povezivanje osnovnih servisa kojima se može pristupiti putem programa Microsoft Graph može utjecati na ukupnu dostupnost i performanse programa Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="78090-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="78090-162">Da biste provjerili stanje servisa Azure Active Directory, provjerite status **sigurnosnih + identifikacijskih** servisa navedenih na [stranici statusa Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="78090-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="78090-163">Za servise sustava Office koji pridonose programu Microsoft Graph provjerite status servisa navedenih na [nadzornoj ploči zdravstvene službe sustava Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="78090-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
