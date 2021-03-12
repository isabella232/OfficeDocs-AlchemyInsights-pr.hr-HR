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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743436"
---
# <a name="create-user"></a>Stvaranje korisnika

**OBAVIJEST**

- [Poništavanje podrške za prijavu na WebView s Googlea u programu Google Počevši od 4 siječanj 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Provjerite utječu li na vaše aplikacije slijedeći [Googleove smjernice](https://go.microsoft.com/fwlink/?linkid=2157323) o kompatibilnosti testiranja.
- Provjerite koristite li web-prikaz sustava ili sistemski preglednik prilikom prijave korisnika pomoću računa potrošača za Google. Dodatne informacije potražite u članku [Problemi s prijavom u aplikacije pomoću preglednika Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Ne mogu stvoriti novog korisnika u direktoriju Azure AD**

1. Provjerite jeste li ovlašteni za stvaranje novog standardnog korisnika. U servisu Azure Active Directory (AD) možete stvoriti novog standardnog korisnika samo za globalne administratore ili ulogu administratora korisnika. Ako niste u jednoj od tih uloga, zatražite od administratora da vas doda u neku od ovih uloga ili da stvori novi korisnički račun za vas.
1. Provjerite je li korisničko ime u domeni koja je potvrđena u servisu Azure AD. Ako nemate potvrđene prilagođene nazive domena u Azure AD-u, možete koristiti početnu domenu Azure AD, koja završava s *. onmicrosoft.com.
1. Provjerite je li korisničko ime u domeni koja se ne šalje na Azure AD iz lokalnog oglasa. Korisnici se ne mogu dodati u oblak s nazivima domena koji su na lokalnoj stranici.
1. Pobrinite se da nijedan drugi korisnik ili kontakt već ima korisničko ime koje želite dodijeliti novom korisniku. Korisnička imena moraju biti jedinstvena na servisu Azure AD.
1. Pogledajte [Azure ad uloge i administratore](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.
1. Pogledajte [nazive domena](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.
1. Pregledajte [zapisnike nadzora](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) da biste vidjeli detaljnije informacije o nedavno stvorenom ili izbrisanom korisniku kao što je taj koji je izvršio akciju i kada.
1. Dodatne informacije o dodavanju novih korisnika potražite u članku [Korištenje portala Azure za stvaranje novog korisnika u Azure ad-u](/azure/active-directory/active-directory-users-create-azure-portal).
1. [Administrativne uloge za Azure ad](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): dozvole za administratorske uloge u servisu Azure Active Directory
1. Možete koristiti i [Azure ad PowerShell da biste stvorili novog korisnika](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
