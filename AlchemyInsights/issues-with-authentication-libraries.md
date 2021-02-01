---
title: Problemi s bibliotekama za provjeru autentičnosti
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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063581"
---
# <a name="issues-with-authentication-libraries"></a>Problemi s bibliotekama za provjeru autentičnosti

1. [Biblioteke za provjeru autentičnosti Microsoftove platforme za dokumente](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) popisuju Microsoftove podržane i kompatibilne biblioteke klijenta i middleware-a.
2. Biblioteka programa Microsoft Authentication (MSAL) podržava nekoliko [tokova provjere autentičnosti](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) za korištenje u različitim scenarijima aplikacija.
3. Da biste provjerili autentičnost i nabavili tokene, inicijalizirajte novu javnu ili povjerljivu klijentske aplikacije u kodu. Prilikom inicijalizacije klijentske aplikacije u biblioteci Microsoft Authentication (MSAL) možete postaviti nekoliko mogućnosti konfiguracije. Dodatne informacije potražite u članku [mogućnosti konfiguracije aplikacije](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Kraj podrške za Azure Active Directory za biblioteku autentičnosti (ADAL) i Azure AD Graph API (AAD Graph)**

**Počevši od 30 lipnja 2020**, više nećemo dodavati nove značajke u AD Graph Adal i Azure. I dalje ćemo pružati tehničku podršku i sigurnosna ažuriranja, ali više nećemo pružati ažuriranja značajki.

**Počevši od 30 lipnja 2022**, završit ćemo podršku za Adal i Azure ad Graph i više neće pružati tehničku podršku ni Sigurnosno ažuriranje.

Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće *dobiti nikakvu tehničku podršku ni Sigurnosno ažuriranje*.

Aplikacije koje koriste Azure AD Graph nakon tog vremena možda više neće primati odgovore iz krajnjih točaka Azure AD Graph.

**ADAL migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) koja ima najnovije značajke i sigurnosna ažuriranja.

Ako koristite Microsoftove aplikacije, znajte da je Microsoft u postupku migracije svojih aplikacija u MSAL uz krajnji rok za potporu, čime će se osigurati da koristi MSAL-ove trajne sigurnosti i poboljšanja značajki.

Dodatne informacije potražite u članku:

1. [Pročitajte najčešća pitanja vezana za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saznajte kako migrirati aplikacije na platformu](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL, preporučujemo vam da pregledate sve izvorne šifre aplikacija i ako je primjenjivo, obratite se svim pružateljima programa ISVs ili aplikacije. Microsoftova podrška također vam može pružiti popis svih aplikacija koje nisu Microsoftove ADAL u vašem klijentu.

**Migracija grafikona AAD**

Za aplikacije koje koriste Azure AD Graph, slijedite upute da biste [migrirali aplikacije Azure ad Graph u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Naš popis za migraciju sadrži točku početka.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Vaš portal za registraciju Azure aplikacija prikazuje koje aplikacije koriste AAD Graph. Preporučujemo da pregledate izvorni kod svih aplikacija i ako je primjenjivo obratite se svim ISV-ovima ili davateljima aplikacija. Microsoftova podrška može vam pružiti i popis svih korištenja AAD grafikona u vašem zakupcu.
3. Da bi aplikacija pristupio podacima u programu Microsoft Graph, korisnik ili administrator mora mu dodijeliti ispravne dozvole putem postupka pristanka. [Referenca dozvola za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) prikazuje popise dozvola povezanih sa svakim glavnim skupom programa Microsoft Graph Apis. Nudi i upute za korištenje dozvola.
