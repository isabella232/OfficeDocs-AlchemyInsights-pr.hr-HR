---
title: Problemi s bibliotekama provjere autentičnosti
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54027996"
---
# <a name="issues-with-authentication-libraries"></a>Problemi s bibliotekama provjere autentičnosti

1. [Microsoftova platforma za identitete provjere autentičnosti navode](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) biblioteke klijenata i srednjih programa koje podržava Microsoft.
2. Microsoftova biblioteka provjere autentičnosti (MSAL) podržava nekoliko [tijekova provjere autentičnosti](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) za korištenje u različitim scenarijima aplikacije.
3. Da biste provjerili autentičnost i dobili tokene, u kodu inicijalizirate novu javnu ili povjerljivu klijentske aplikacije. Prilikom inicijalizacije klijentske aplikacije u biblioteci Microsoftove provjere autentičnosti (MSAL) možete postaviti nekoliko mogućnosti konfiguracije. Dodatne informacije potražite u članku [Mogućnosti konfiguracije aplikacije](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Kraj podrške za Azure Active Directory provjere autentičnosti (ADAL) i AZURE AD Graph API (AAD Graph)**

**Od 30. lipnja 2020.** više nećemo dodavati nove značajke u ADAL i Azure AD Graph. I dalje ćemo pružati tehničku podršku i sigurnosna ažuriranja, ali više nećemo pružati ažuriranja značajki.

**Od 30. lipnja 2022.** završit ćemo podršku za ADAL i Azure AD Graph i više nećemo pružati tehničku podršku ni sigurnosna ažuriranja.

Aplikacije koje koriste ADAL u postojećim verzijama operacijskog sustava i dalje će funkcionirati nakon tog vremena, ali neće dobiti *tehničku podršku ni sigurnosna ažuriranja*.

Aplikacije koje koriste Azure AD Graph nakon tog vremena možda više neće primati odgovore od krajnje točke servisa Azure AD Graph.

**ADAL migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) koja ima najnovije značajke i sigurnosna ažuriranja.

Ako koristite Microsoftove aplikacije, znaj da Je Microsoft u tijeku s migriranjem aplikacija u MSAL do krajnjeg roka podrške, čime se jamči da će imati koristi od trajnih poboljšanja sigurnosti i značajki MSAL-a.

Dodatne informacije potražite u sljedećim člancima:

1. [Pročitajte najčešća pitanja vezana za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saznajte kako migrirati aplikacije na platformu](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL, preporučujemo da pregledate izvorni kod svih aplikacija i, ako je primjenjivo, kontaktirate bilo kojeg DAVATELJa internetskih usluga ili davatelja aplikacija. Microsoftova podrška također vam može pružiti popis svih aplikacija koje nisu Microsoftove ADAL u vašem klijentu.

**Migracija grafikona AAD**

Za aplikacije koje koriste Azure AD Graph slijedite naše [smjernice za migriranje](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)aplikacija Azure AD Graph u Microsoft Graph .

1. [Naš kontrolni popis za migraciju daje točku za početak rada.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Vaš portal za registraciju Azure aplikacija prikazuje koje aplikacije koriste AAD Graph. Preporučujemo da pregledate izvorni kod svih aplikacija i ako je primjenjivo obratite se svim ISV-ovima ili davateljima aplikacija. Microsoftova podrška može vam pružiti i popis svih Graph AAD-a u klijentu.
3. Da bi vaša aplikacija pristupala podacima u aplikaciji Microsoft Graph, korisnik ili administrator moraju mu dodijeliti odgovarajuće dozvole putem postupka pristanka. Referenca [dozvola za Microsoft Graph sadrži](https://docs.microsoft.com/graph/permissions-reference) popis dozvola povezanih sa svakim glavnim skupom API-ja Graph Microsofta. Sadrži i smjernice za korištenje dozvola.
