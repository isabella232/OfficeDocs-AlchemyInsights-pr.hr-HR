---
title: Nabavite popis enterprise aplikacija
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404332"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="6a318-102">Nabavite popis enterprise aplikacija</span><span class="sxs-lookup"><span data-stu-id="6a318-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="6a318-103">Da **biste dobili popis** korporacijskih aplikacija (sve aplikacije ili filtrirane zaslonskim imenom, ID-om, IDENTIFIKATOR-om itd.) putem naredbe Powershell, pogledajte [get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="6a318-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="6a318-104">Da biste dobili popis glavnih objekata servisa (svih objekata ili filtriranih prema ID-u) putem naredbe Powershell, pogledajte [get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="6a318-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="6a318-105">Ako želite dobiti **popis aplikacija konfiguriranih za SAML,** sljedeće skripte komponente PowerShell mogu vam pomoći:</span><span class="sxs-lookup"><span data-stu-id="6a318-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="6a318-106">Svaka aplikacija bilo da je to aplikacija OAuth ili SAML aplikacija (i galerija i aplikacije koje nisu galerije) imaju dva objekta stvorena u AAD-u kada se njihova registracija dogodi.</span><span class="sxs-lookup"><span data-stu-id="6a318-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="6a318-107">Jedan se zove objekt aplikacije, a drugi objekt Upravitelj servisa.</span><span class="sxs-lookup"><span data-stu-id="6a318-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="6a318-108">Kada svojstva objekta Upravitelj servisa odbacite pomoću komponente PowerShell, pronaći ćete da svaka aplikacija ima određeni broj oznaka povezanih s njim kao što su:</span><span class="sxs-lookup"><span data-stu-id="6a318-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="6a318-109">OAuth aplikacije imaju oznaku pod nazivom **"WindowsAzureActiveDirectoryIntegratedApp"**</span><span class="sxs-lookup"><span data-stu-id="6a318-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="6a318-110">Galerija SAML aplikacije ima oznaku pod nazivom **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="6a318-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="6a318-111">Saml aplikacije koje nisu galerije imaju oznaku pod nazivom **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="6a318-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="6a318-112">Stoga možete koristiti te oznake i saznati koja je to aplikacija.</span><span class="sxs-lookup"><span data-stu-id="6a318-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="6a318-113">Oznaka **"WindowsAzureActiveDirectoryIntegratedApp"** uobičajena je za sve vrste aplikacija.</span><span class="sxs-lookup"><span data-stu-id="6a318-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="6a318-114">Pomoću sljedećeg isječka možete popisati sve SAML aplikacije (i galeriju i ne-galeriju):</span><span class="sxs-lookup"><span data-stu-id="6a318-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="6a318-115">Dodatne informacije potražite u članku Prepoznavanje [aplikacija s omogućenim SAML-om na servisu Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span><span class="sxs-lookup"><span data-stu-id="6a318-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="6a318-116">**Traženje i popis samo web-aplikacija:** koristite naredbu u nastavku da biste sve aplikacije azure AD dobili s vrstom aplikacije "Web app/API" (Web-aplikacija/API)</span><span class="sxs-lookup"><span data-stu-id="6a318-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="6a318-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="6a318-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="6a318-118">**Samo pronađite i na popisu Nativne** aplikacije: pokrenite sljedeću naredbu da biste dobili sve nativne klijentske (stolno/mobilne uređaje) aplikacije.</span><span class="sxs-lookup"><span data-stu-id="6a318-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="6a318-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="6a318-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="6a318-120">**Izvoz svih registriranih pojedinosti aplikacije Azure AD u CSV:** naredba u nastavku izvozi sve aplikacije Azure AD s obaveznim detaljima u csv datoteku:</span><span class="sxs-lookup"><span data-stu-id="6a318-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="6a318-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, Logouturl |</span><span class="sxs-lookup"><span data-stu-id="6a318-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="6a318-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="6a318-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="6a318-123">**Potrebno je izvesti popis neiskorištenih aplikacija sustava Azure** – izvješće o nadzoru</span><span class="sxs-lookup"><span data-stu-id="6a318-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="6a318-124">Azure AD može prikazati zapisnike aplikacija samo do 30 dana ako imate licencu za Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="6a318-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="6a318-125">Imate dvije mogućnosti zadržavanja podataka dulje od 30 dana.</span><span class="sxs-lookup"><span data-stu-id="6a318-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="6a318-126">API-jem [za izvješćivanje servisa Azure AD možete](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) dohvatiti podatke programski i pohraniti ih u bazu podataka.</span><span class="sxs-lookup"><span data-stu-id="6a318-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="6a318-127">Možete i integrirati zapisnike nadzora u sustav SIEM drugog proizvođača.</span><span class="sxs-lookup"><span data-stu-id="6a318-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="6a318-128">Popis aplikacija možete preuzeti i za sve aplikacije i aplikacije u vlasništvu u odjeljku Azure Active directory>Registracije aplikacija>Preuzmi>Sve aplikacije/aplikacije u vlasništvu.</span><span class="sxs-lookup"><span data-stu-id="6a318-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="6a318-129">Da biste dobili popis aplikacija putem programa MS Graph, pogledajte popis aplikacija [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) i vrsta resursa aplikacije [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="6a318-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
