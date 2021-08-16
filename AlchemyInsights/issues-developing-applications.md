---
title: Problemi s razvojem aplikacija
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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013416"
---
# <a name="issues-developing-applications"></a>Problemi s razvojem aplikacija

Da biste otklonili najčešće probleme prilikom Azure Active Directory (AD) aplikacija, pogledajte sljedeće članke:

- [Ne mogu se prijaviti u aplikacije samo pomoću preglednika Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Ne znam kako promijeniti zadane postavke životnog ciklusa tokena za moju aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Ja sam zbunjen o tome kako funkcionira pristanak aplikacije](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Ne znam kako dodijeliti dozvole za aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Ne razumijem razliku između ovlaštenih i dozvola za aplikacije](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Kraj podrške za Azure Active Directory provjere autentičnosti (ADAL) i AZURE AD Graph API (AAD Graph)***

- Od 30. lipnja 2020. više nećemo dodavati nove značajke u Azure Active Directory Authentication Library (ADAL) i Azure AD Graph API (AAD Graph). I dalje ćemo pružati tehničku podršku i sigurnosna ažuriranja, ali više nećemo pružati ažuriranja značajki.

- Od 30. lipnja 2022. ukinut ćemo podršku za ADAL i AAD Graph i više nećemo pružati tehničku podršku ili sigurnosna ažuriranja. Zbog tog uvjeta sljedeće su implikacije:

    - Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće dobiti nikakvu tehničku podršku ili sigurnosna ažuriranja.

    - Aplikacije koje koriste AAD Graph nakon tog vremena možda više neće primati odgovore od krajnje točke Graph AAD

**ADAL migracija**

Ako koristite Microsoftove aplikacije, preporučujemo ažuriranje na Microsoftovu biblioteku za provjeru autentičnosti (MSAL), koja sadrži najnovije značajke i sigurnosna ažuriranja. Ova je preporuka u kontekstu microsoftova pokretanja postupka migracije aplikacija u MSAL do krajnjeg roka za podršku. 

Migracija microsoftovih aplikacija u MSAL jamči da će aplikacije imati koristi od trajnih poboljšanja sigurnosti i značajki servisa MSAL.

1. [Pročitajte najčešća pitanja vezana za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Saznajte kako migrirati aplikacije na platformu](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL, preporučujemo da pregledate izvorni kod svih aplikacija i, ako je primjenjivo, kontaktirate neovisne proizvođače softvera (ISV-ove) ili davatelje aplikacija. Microsoftova podrška također vam može pružiti popis svih aplikacija koje nisu Microsoftove ADAL u vašem klijentu.

**Migracija grafikona AAD**

Za aplikacije koje koriste AAD Graph slijedite naše smjernice za migriranje AAD Graph aplikacija u Microsoft Graph:

1. [Naš popis za migraciju pruža točku početka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Vaš portal za registraciju Azure aplikacija prikazuje koje aplikacije koriste AAD Graph. Preporučujemo da pregledate izvorni kod svih aplikacija i, ako je primjenjivo, kontaktirate neovisne proizvođače softvera (ISV-ove) ili davatelje aplikacija. Microsoftova podrška može vam pružiti i informacije o korištenju Graph AAD-a u klijentu.







