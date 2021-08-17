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
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116720"
---
# <a name="get-a-list-of-enterprise-applications"></a>Nabavite popis enterprise aplikacija

1. Da **biste dobili popis** korporacijskih aplikacija (sve aplikacije ili filtrirane zaslonskim imenom, ID-om, IDENTIFIKATOR-om itd.) putem naredbe Powershell, pogledajte [get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Da biste dobili popis glavnih objekata servisa (svih objekata ili filtriranih prema ID-u) putem naredbe Powershell, pogledajte [get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Ako želite dobiti **popis aplikacija konfiguriranih za SAML,** sljedeće skripte komponente PowerShell mogu vam pomoći:

    Svaka aplikacija bilo da je to aplikacija OAuth ili SAML aplikacija (i galerija i aplikacije koje nisu galerije) imaju dva objekta stvorena u AAD-u kada se njihova registracija dogodi. Jedan se zove objekt aplikacije, a drugi objekt Upravitelj servisa. Kada svojstva objekta Upravitelj servisa odbacite pomoću komponente PowerShell, pronaći ćete da svaka aplikacija ima određeni broj oznaka povezanih s njim kao što su:

    - OAuth aplikacije imaju oznaku pod nazivom **"WindowsAzureActiveDirectoryIntegratedApp"**
    - Galerija SAML aplikacije ima oznaku pod nazivom **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Saml aplikacije koje nisu galerije imaju oznaku pod nazivom **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Stoga možete koristiti te oznake i saznati koja je to aplikacija. Oznaka **"WindowsAzureActiveDirectoryIntegratedApp"** uobičajena je za sve vrste aplikacija. Pomoću sljedećeg isječka možete popisati sve SAML aplikacije (i galeriju i ne-galeriju):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Dodatne informacije potražite u članku Prepoznavanje [aplikacija s omogućenim SAML-om na servisu Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Traženje i popis samo web-aplikacija:** koristite naredbu u nastavku da biste sve aplikacije azure AD dobili s vrstom aplikacije "Web app/API" (Web-aplikacija/API)

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Samo pronađite i na popisu Nativne** aplikacije: pokrenite sljedeću naredbu da biste dobili sve nativne klijentske (stolno/mobilne uređaje) aplikacije.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Izvoz svih registriranih pojedinosti aplikacije Azure AD u CSV:** naredba u nastavku izvozi sve aplikacije Azure AD s obaveznim detaljima u csv datoteku:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, Logouturl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Potrebno je izvesti popis neiskorištenih aplikacija sustava Azure** – izvješće o nadzoru

    Azure AD može prikazati zapisnike aplikacija samo do 30 dana ako imate licencu za Azure AD premium.
    Imate dvije mogućnosti zadržavanja podataka dulje od 30 dana. API-jem [za izvješćivanje servisa Azure AD možete](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) dohvatiti podatke programski i pohraniti ih u bazu podataka. Možete i integrirati zapisnike nadzora u sustav SIEM drugog proizvođača.

    Popis aplikacija možete preuzeti i za sve aplikacije i aplikacije u vlasništvu u odjeljku Azure Active directory>Registracije aplikacija>Preuzmi>Sve aplikacije/aplikacije u vlasništvu.

    Da biste dobili popis aplikacija putem servisa MS Graph, pogledajte članak Popis [aplikacija – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) i vrsta resursa [aplikacije – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
