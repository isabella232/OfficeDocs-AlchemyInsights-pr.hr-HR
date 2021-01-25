---
title: Problemi u razvoju aplikacija
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974230"
---
# <a name="issues-developing-applications"></a>Problemi u razvoju aplikacija

Da biste otklonili poteškoće s najčešćih problema prilikom izgradnje aplikacija Azure Active Directory (AD), pročitajte sljedeće članke:

- [Vidim poteškoće prilikom prijave u aplikacije pomoću preglednika Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Ne znam kako promijeniti zadane vrijednosti trajanja tokena za moju aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Zbunjen sam o tome kako funkcionira suglasnost aplikacija](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Ne znam kako dodijeliti dozvole za svoju aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Ne razumijem razliku između dozvola delegiranih i aplikacija](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Kraj podrške za Azure Active Directory za biblioteku autentičnosti (ADAL) i Azure ad Graph API (AAD Graph)** _

- Počevši od 30 Lipanj, 2020, više nećemo dodavati nove značajke u biblioteku servisa Azure Active Directory za provjeru autentičnosti (ADAL) i API-ja za Azure AD Graph (AAD Graph). Nastavit ćemo pružati tehničku podršku i sigurnosno ažuriranje, ali više nećemo pružati ažuriranja značajki.

- Počevši od 30 lipnja 2022, završit ćemo podršku za ADAL i AAD Graph i više neće pružati tehničku podršku ni Sigurnosno ažuriranje. Kao rezultat tog stanja, slijede implikacije:

    - Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće dobiti nikakvu tehničku podršku ni Sigurnosno ažuriranje.

    - Aplikacije koje koriste AAD Graph nakon tog vremena možda više neće primati odgovore iz krajnje točke AAD grafikona

_ *Adal migracija**

Ako koristite Microsoftove aplikacije, preporučujemo ažuriranje Microsoftove biblioteke za provjeru autentičnosti (MSAL), koja sadrži najnovije značajke i sigurnosno ažuriranje. Ta je preporuka u kontekstu programa Microsoft koji pokreće postupak migracije aplikacija u MSAL uz krajnji rok podrške. 

Migracija Microsoftova aplikacija u MSAL jamči da će aplikacije imati koristi od aktualnih sigurnosti i poboljšanja značajki MSAL-a.

1. [Pročitajte najčešća pitanja o dodatku](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Informacije o migraciji aplikacija na temelju osnove platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ako vam je potrebna pomoć u razumijevanju koja aplikacija koristi ADAL, preporučujemo vam da pregledate sve izvorne šifre aplikacija i, ako je moguće, dostupate do svih neovisnih proizvođača softvera (ISVs) ili davatelja aplikacija. Microsoftova podrška može vam pružiti i popis svih aplikacija koje nisu Microsoftove ADAL u vašem zakupcu.

**Migracije grafikona AAD**

Za aplikacije koje koriste AAD Graph, slijedite upute da biste migrirali aplikacije AAD Graph u Microsoft Graph:

1. [Naš popis za migraciju sadrži točku početka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Portal za registraciju servisa Azure sadrži programe koje koristi AAD Graph. Preporučujemo da pregledate sve izvorne šifre aplikacija i, ako je primjenjivo, dođete do svih neovisnih proizvođača softvera (ISVs) ili davatelja aplikacija. Microsoftova podrška omogućuje vam i informacije o korištenju AAD grafikona u vašem zakupcu.







