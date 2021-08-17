---
title: Brisanje i vraćanje aplikacija
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
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102563"
---
# <a name="delete-or-restore-applications"></a>Brisanje i vraćanje aplikacija

**Brisanje aplikacije s klijenta servisa Azure AD:**

1. Na **portalu Azure AD** odaberite **Korporacijske aplikacije**. Zatim pronađite i odaberite aplikaciju koju želite izbrisati.
2. U **odjeljku Upravljanje** u lijevom oknu odaberite **Svojstva**.
3. Odaberite **Izbriši**, a zatim **Da** da biste potvrdili da želite izbrisati aplikaciju s klijenta servisa Azure AD.

Dodatne informacije o brisanju aplikacije potražite u članku Brzi početak rada: Brisanje aplikacije [s klijenta servisa Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

U ljuski PowerShell cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) uklanja konfiguracije proxyja aplikacije iz određene aplikacije u programu Azure Active Directory i može potpuno izbrisati aplikaciju ako je to navedeno.

Izbrisanu **aplikaciju možete vratiti pomoću** komponente PowerShell. Kada prepoznate aplikaciju koju želite vratiti, možete je vratiti pomoću [značajke Vraćanje-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
