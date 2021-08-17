---
title: Traženje aplikacija koje nedostaju na lopatici za registraciju aplikacije
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
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057094"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Traženje aplikacija koje nedostaju na lopatici za registraciju aplikacije

1. Nije moguće pronaći aplikacije na portalu za registraciju aplikacija.

    Ako je aplikacija aplikacija s više klijenta i registrirana je na drugom klijentu, ona se neće prikazati u odjeljku Registracija aplikacije. No možda ćete ga pronaći u odjeljku Enterprise Applications blade kada mu se pristupi (nakon pristanka) i upravitelj servisa bude stvoren na vašem klijentu. Dodatne informacije potražite u članku [Upravitelji & servisa na servisu Azure AD – Microsoftova platforma za identitete](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Nije moguće prikazati aplikacije na alatu za registraciju aplikacija iako ste administrator.

    Provjerite nalazite li se u pravom direktoriju na portalu Azure.
3. Moja aplikacija nije navedena u odjeljku Enterprise Applications blade, ali se prikazuje prilikom upita naredbe PowerShell.

    Ponekad se nakon brisanja aplikacije s portala Azure ne prikazuje na portalu, ali možda nije potpuno izbrisana. Dodatne informacije potražite u sljedećim člancima:
    - Popis prethodno izbrisanih aplikacija možete dohvatiti i vidjeti prikazuje li se aplikacija na popisu pomoću naredbe Powershell: **Get-AzureADDeletedApplication**. Dodatne informacije potražite u članku [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Ako aplikaciju želite u potpunosti ukloniti, pokušajte sljedeće u ljuski PowerShell: **Remove-AzureADApplication -ObjectId**. Dodatne informacije potražite u članku [Uklanjanje AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Možete i pokušati vratiti izbrisanu aplikaciju pomoću sljedeće naredbe ljuske Powershell: **Vraćanje značajke AzureADDeletedApplication -ObjectId**. Dodatne informacije potražite u članku [Vraćanje-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Popis svih unaprijed instaliranih korporacijskih aplikacija nije moguće pronaći u novom klijentu servisa Azure.

    Ne postoje unaprijed instalirane korporacijske aplikacije na servisu Azure AD po zadanom. Morate je dodati ručno iz mogućnosti "Nova aplikacija" tako da je pregledavate iz galerije azure AD ili dodate aplikaciju koja nije galerija. Dodatne informacije potražite u članku [Brzi početak rada: dodavanje aplikacije na klijent Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Ako ste globalni administrator, aplikacijama možete jednostavno pristupiti pomoću pokretača [aplikacija Microsoft 365 aplikacije](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Nije moguće pronaći aplikacije s portala Moje aplikacije.

    Provjerite nisu li aplikacije skrivene na stranici zbirke moje aplikacije. Dodatne informacije potražite u članku [Zbirke (pretpregled) na portalu Moje aplikacije – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Da biste pokrenuli aplikacije s portala Moje aplikacije, pogledajte & potražite u članku Pronalaženje aplikacija na portalu Moje [aplikacije – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Office 365 Aplikacija Mover ne prikazuje se na oštrici Enterprise Applications nakon instalacije.

    Aplikacija "Office 365 Mover" aplikacija je za više korisnika koja se ne mora dodati u AAD pomoću odjeljka Galerija aplikacija u odjeljku Registracija korporacijskih aplikacija. Da biste Office 365 aplikaciji Mover, jednostavno se prijavite u aplikaciju i zatražit će pristanak korisnika za dozvole. Kada korisnik pruži pristanak, ta će se aplikacija automatski dodati klijentu s ID-om e-pošte koji ste prijavili.

    Nakon prijave u aplikaciju trebali biste moći pronaći unos aplikacije ispod oštrice enterprise aplikacija u AAD-u. Tu aplikaciju morate potražiti tako da upišete puno ime i prezime, npr. "Office 365 Mover" ili jednostavno pretražite "office" i ona bi trebala biti na popisu aplikacije. Dodatne informacije potražite u [članku Office 365 Mover kaže da](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)je već instaliran, ali nije naveden u galeriji Enterprise Application .
8. Brzi početak: prikaz popisa aplikacija koje koriste [klijent sustava Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) za upravljanje identitetom pokazuje kako prikazati aplikacije, poznate i kao aplikacije, koje su već postavljene za korištenje klijenta azure AD kao davatelja identiteta (IDP).
9. [Otklanjanje poteškoća prilikom dodavanja ili uklanjanja aplikacije u Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) pomoći će vam da shvatite uobičajene probleme s kojima se osobe suočavaju s prikazom aplikacija Azure Active Directory.
