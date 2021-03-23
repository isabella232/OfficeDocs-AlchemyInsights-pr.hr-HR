---
title: Problemi s upravljanjem korisničkim korisnicima
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035137"
---
# <a name="user-management-issues"></a>Problemi s upravljanjem korisničkim korisnicima

**Što se događa s trenutnim dodijeljenim korisnicima u aplikaciji ako Onemogućujem svojstvo "potreban je korisnički zadatak" (postavljanje ovog svojstva na ne)?**

Onemogućivanje **obaveznog korisničkog zadatka** ne utječe na trenutno dodijeljene korisnike. Onemogućivanjem tog svojstva svim će korisnicima dopustiti pristup aplikaciji. Svi navedeni korisnici i korisnici dodijeljeni grupama u aplikaciji i dalje će biti valjani.

- Da biste aplikaciju ograničili na određeni skup korisnika, pročitajte članak [ograničenje aplikacije Azure ad na skup korisnika – Microsoftova platforma identiteta | Microsoftovi dokumenti](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Da biste korisnike i grupe dodijelili korporativnim aplikacijama u servisu Azure Active Directory (Azure AD), na portalu Azure ili pomoću komponente PowerShell, pročitajte članak [Upravljanje zadatkom korisnika za aplikaciju u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Da biste delegiraju dozvole za stvaranje i upravljanje aplikacijama, pogledajte odjeljak [delegiranje administratorskih dozvola za upravljanje aplikacijama-Azure ad | Microsoftovi dokumenti](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Sakrivanje određenih korporacijskih aplikacija od korisnika** – slijedite korake u nastavku da biste skrivali sve aplikacije sustava Microsoft 365 na ploči **myapps** . Aplikacije će i dalje biti vidljive na portalu sustava Office 365.

 1. Prijavite se na portal Azure kao globalni administrator za svoj direktorij. 
 2. Odaberite **Azure Active Directory**. 
 3. Odaberite **korisnici**. 
 4. Odaberite **korisničke postavke**. 
 5. U odjeljku **Enterprise aplikacije** kliknite **upravljanje načinom na koji krajnji korisnici pokrenu i pregledavaju njihove aplikacije**. 
 6. Da bi **korisnici mogli vidjeti samo aplikacije sustava office 365 na portalu sustava office 365**, kliknite **da**. 
 7. Kliknite **Spremi**. 
 8. Dodatne informacije potražite u članku [sakrivanje korporacijske aplikacije iz korisničkog iskustva u servisu Azure ad | Microsoftovi dokumenti](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Ako u mnoge tvrtke ili ustanove nudite softver kao aplikaciju servisa (SaaS), aplikaciju možete konfigurirati tako da prihvaća prijave iz bilo kojeg stanara Azure Active Directory (Azure AD). Ta se konfiguracija naziva "upućivanje u multi-stanar aplikacije". Korisnici u bilo kojem klijentu za Azure AD bit će u mogućnosti prijaviti se u aplikaciju nakon pristanka da koriste svoj račun uz vašu aplikaciju. Dodatne informacije potražite u članku [Sastavljanje aplikacija koje se prijave u korisnike servisa Azure ad-Microsoft Identity Platform | Microsoftovi dokumenti](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Kako krajnji korisnik može pristupiti aplikaciji kada je dodijeljen aplikaciji?**

Svaka aplikacija u aplikaciji Enterprise Application sječiva sadrži vezu za krajnje korisnike za pristup. Korisnici mogu i na jednostavan način pristupati aplikaciji putem portala **Myapps** .

- **Želite li znati koje su aplikacije i vrste aplikacija korištene od strane korisnika?**

Izvješća za prijavu možete preuzeti zadnjih 30 dana iz **portal.azure.com > Azure Active directory> Signins> preuzimanje izvješća**.

- Upute za [dodjelu pristanka korisnika Wide administratore u aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) i [Konfiguriranje pristanka krajnjih klijenata na aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Razumijevanje [načina funkcioniranja pristanka](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) i [Upravljanje pristankom na aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


