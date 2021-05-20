---
title: Stvaranje korisnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569703"
---
# <a name="create-user"></a>Stvaranje korisnika

**NAJAVA:**

- [Deprecation of WebView sign-in support from Google starting 4 siječnja 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Provjerite mogu li na vaše aplikacije utjecati Googleove [smjernice za](https://go.microsoft.com/fwlink/?linkid=2157323) testiranje kompatibilnosti.
- Provjerite koristite li web-prikaz sustava ili preglednik sustava prilikom prijave korisnika pomoću korisničkih Google računa. Dodatne informacije potražite u članku [Problemi prilikom prijave u aplikacije samo u pregledniku Chrome](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Ne mogu stvoriti novog korisnika u direktoriju servisa Azure AD**

1. Provjerite jeste li ovlašteni za stvaranje novog standardnog korisnika. Samo uloga globalnog administratora ili administratora korisnika u programu Azure Active Directory (AD) može stvoriti novog standardnog korisnika. Ako niste u jednoj od tih uloga, zatražite od administratora da vas doda u jednu od tih uloga ili da vam stvori novi korisnički račun.
1. Provjerite nalazi li se korisničko ime u domeni potvrđenoj u servisu Azure AD. Ako na servisu Azure AD nema potvrđenih prilagođenih naziva domena, možete koristiti početnu domenu servisa Azure AD, koja završava s *.onmicrosoft.com.
1. Provjerite je li korisničko ime u domeni koja nije pridružena servisu Azure AD iz lokalnog AD-a. Korisnike nije moguće dodati u oblak s nazivima domena koji su pridruženi lokalno.
1. Provjerite ima li nijedan drugi korisnik ili kontakt korisničko ime koje želite dodijeliti novom korisniku. Korisnička imena moraju biti jedinstvena na servisu Azure AD.
1. Pogledajte [uloge i administratore servisa Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.
1. Pogledajte [nazive domena za](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.
1. Pregledajte [zapisnike nadzora](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) da biste vidjeli detaljnije informacije o nedavno stvorenom ili izbrisanom korisniku, npr. o tome tko je izveo akciju i kada.
1. Dodatne informacije o dodavanju novih korisnika potražite u članku Stvaranje novog korisnika na [servisu Azure AD](/azure/active-directory/active-directory-users-create-azure-portal)pomoću portala Azure .
1. [Administratorske uloge servisa Azure AD](/azure/active-directory/active-directory-assign-admin-roles): administratorske dozvole za Azure Active Directory
1. Da biste stvorili [novog korisnika, možete koristiti](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)i Azure AD PowerShell .
