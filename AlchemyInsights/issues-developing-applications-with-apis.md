---
title: Problemi s razvojem aplikacija s API-jem
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013452"
---
# <a name="issues-developing-applications-with-apis"></a>Problemi s razvojem aplikacija s API-jem

Da biste počeli koristiti API Azure Active Directory Graph, pogledajte vodič za brzo pokretanje [api-ja](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) za Azure AD Graph ili pogledajte interaktivnu dokumentaciju reference [za Azure AD Graph API.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Kraj podrške za Azure Active Directory provjere autentičnosti (ADAL) i AZURE AD Graph API (AAD Graph)**

**Od 30. lipnja 2020.** više nećemo dodavati nove značajke u ADAL i Azure AD Graph. I dalje ćemo pružati tehničku podršku i sigurnosna ažuriranja, ali više nećemo pružati ažuriranja značajki.

**Od 30. lipnja 2022.** završit ćemo podršku za ADAL i Azure AD Graph i više nećemo pružati tehničku podršku ni sigurnosna ažuriranja.

Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće dobiti nikakvu tehničku podršku ili sigurnosna ažuriranja.

Aplikacije koje koriste Azure AD Graph nakon tog vremena možda više neće primati odgovore od krajnje točke servisa Azure AD Graph.

**ADAL migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) koja ima najnovije značajke i sigurnosna ažuriranja.

Ako koristite Microsoftove aplikacije, znaj da Je Microsoft u tijeku s migriranjem aplikacija u MSAL do krajnjeg roka podrške, čime se jamči da će imati koristi od trajnih poboljšanja sigurnosti i značajki MSAL-a.

1. [Pročitajte najčešća pitanja o ADAL-u.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Saznajte kako migrirati aplikacije po platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL, preporučujemo da pregledate izvorni kod svih aplikacija i, ako je primjenjivo, kontaktirate bilo kojeg DAVATELJa internetskih usluga ili davatelja aplikacija. Microsoftova podrška također vam može pružiti popis svih aplikacija koje nisu Microsoftove ADAL u vašem klijentu.

**Migracija grafikona AAD**

Za aplikacije koje koriste Azure AD Graph slijedite naše smjernice za migriranje aplikacija [Azure AD Graph u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Naš popis za migraciju pruža točku početka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Vaš portal za registraciju Azure aplikacija prikazuje koje aplikacije koriste AAD Graph. Preporučujemo da pregledate izvorni kod svih aplikacija i ako je primjenjivo obratite se svim ISV-ovima ili davateljima aplikacija. Microsoftova podrška može vam pružiti i popis svih Graph AAD-a u klijentu.
1. Da bi vaša aplikacija pristupala podacima u aplikaciji Microsoft Graph, korisnik ili administrator moraju mu dodijeliti odgovarajuće dozvole putem postupka pristanka. Referenca [dozvola za Microsoft Graph sadrži](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) popis dozvola povezanih sa svakim glavnim skupom API-ja Graph Microsofta. Sadrži i smjernice za korištenje dozvola.
