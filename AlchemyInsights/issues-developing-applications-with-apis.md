---
title: Problemi u razvoju aplikacija s API-Jima
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974263"
---
# <a name="issues-developing-applications-with-apis"></a>Problemi u razvoju aplikacija s API-Jima

Da biste započeli korištenje API-ja za Azure Active Directory, pogledajte [priručnik za Azure ad Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) (brz početak rada) ili pogledajte [dokumentaciju o referenci API-ja za interaktivne Azure ad Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Kraj podrške za Azure Active Directory za biblioteku autentičnosti (ADAL) i Azure AD Graph API (AAD Graph)**

**Počevši od 30 lipnja 2020**, više nećemo dodavati nove značajke u AD Graph Adal i Azure. Nastavit ćemo pružati tehničku podršku i sigurnosno ažuriranje, ali više nećemo pružati ažuriranja značajki.

**Počevši od 30 lipnja 2022**, završit ćemo podršku za Adal i Azure ad Graph i više neće pružati tehničku podršku ni Sigurnosno ažuriranje.

Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće dobiti nikakvu tehničku podršku ni Sigurnosno ažuriranje.

Aplikacije koje koriste Azure AD Graph nakon tog vremena možda više neće primati odgovore iz krajnjih točaka Azure AD Graph.

**ADAL migracija**

Preporučujemo ažuriranje [Microsoftove biblioteke za provjeru autentičnosti (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), koja sadrži najnovije značajke i sigurnosno ažuriranje.

Ako koristite Microsoftove aplikacije, znajte da je Microsoft u postupku migracije svojih aplikacija u MSAL uz krajnji rok za potporu, čime će se osigurati da koristi MSAL-ove trajne sigurnosti i poboljšanja značajki.

1. [Pročitajte najčešća pitanja o dodatku](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Saznajte kako migrirati aplikacije na osnovi po platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL, preporučujemo vam da pregledate sve izvorne šifre aplikacija i ako je primjenjivo, obratite se svim pružateljima programa ISVs ili aplikacije. Microsoftova podrška može vam pružiti i popis svih aplikacija koje nisu Microsoftove ADAL u vašem zakupcu.

**Migracije grafikona AAD**

Za aplikacije koje koriste Azure AD Graph, slijedite upute da biste migrirali [aplikacije Azure ad Graph u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Naš popis za migraciju sadrži točku početka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Portal za registraciju servisa Azure sadrži programe koje koristi AAD Graph. Preporučujemo vam da pregledate sve izvorne šifre aplikacija, a ako je primjenjivo, obratite se svim pružateljima programa ISVs ili aplikacije. Microsoftova podrška može vam pružiti i popis svih korištenja AAD grafikona u vašem zakupcu.
1. Da bi aplikacija pristupio podacima u programu Microsoft Graph, korisnik ili administrator mora mu dodijeliti ispravne dozvole putem postupka pristanka. [Referenca dozvola za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) prikazuje popise dozvola povezanih sa svakim glavnim skupom programa Microsoft Graph Apis. Nudi i upute za korištenje dozvola.
