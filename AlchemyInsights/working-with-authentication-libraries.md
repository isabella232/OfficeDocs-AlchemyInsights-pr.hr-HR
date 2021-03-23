---
title: Rad s bibliotekama za provjeru autentičnosti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035016"
---
# <a name="working-with-authentication-libraries"></a>Rad s bibliotekama za provjeru autentičnosti

Da biste riješili problem biblioteke programa Microsoft Authentication (MSAL), učinite sljedeće preporučene korake:

1. **Rad sa programom MSAL**: [biblioteke za provjeru autentičnosti Microsoftove platforme identiteta](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – u ovom se članku sadrži Podrška za biblioteku Microsoft Authentication za nekoliko vrsta aplikacija. Sadrži veze na izvorni kod biblioteke. Gdje nabaviti paket za projekt aplikacije? i podržava li biblioteka korisničke prijave (provjera autentičnosti), pristup zaštićenim web-API-Jima (autorizacija) ili oboje.

2. **Otklanjanje poteškoća s provjerom autentičnosti**: msal podržava nekoliko tokova provjere autentičnosti za korištenje u različitim scenarijima aplikacija. Ovisno o tome kako je vaša klijentska aplikacija izgrađena, MSAL može koristiti jedan ili više tokova provjere autentičnosti koje podržava Microsoftova platforma identiteta. Ovi tijekovi mogu proizvesti nekoliko vrsta tokena i autorizacije, te zahtijevati različite tokene da bi funkcionisali.

3. **Token za Access**: [tokeni za pristup Microsoftovoj platformi za identitete](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -Naučite kako API može provjeriti valjanost i koristiti zahtjeve u pristupnom toknu. Sva dokumentacija u ovom članku, osim ako je navedeno, primjenjuje se samo na tokene izdane za API-je koje ste registrirali. Ne primjenjuje se na tokene izdane za API-je u vlasništvu Microsofta, niti se ti tokeni mogu koristiti za provjeru načina na koji će Microsoftova platforma za identitete izdati žetone za neki API koji ste stvorili.

**Kraj podrške za biblioteku autentičnosti servisa Azure Active Directory (ADAL)**

- **Počevši od 30 lipnja 2020,** više nećemo dodavati nove značajke u AD Graph Adal i Azure. I dalje ćemo pružati tehničku podršku i sigurnosna ažuriranja, ali više nećemo pružati ažuriranja značajki.
- **Počevši od 30 lipnja 2022,** završit ćemo podršku za Adal i Azure ad Graph i više neće pružati tehničku podršku ni Sigurnosno ažuriranje.
- Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće *dobiti nikakvu tehničku podršku ni Sigurnosno ažuriranje*.
- Aplikacije koje koriste Azure AD Graph nakon tog vremena možda više neće primati odgovore iz krajnjih točaka Azure AD Graph.

**ADAL migracija**

- Preporučujemo ažuriranje MSAL-a, koji sadrži najnovije značajke i sigurnosno ažuriranje.
- Ako koristite Microsoftove aplikacije, znajte da je Microsoft u postupku migracije svojih aplikacija u MSAL uz krajnji rok podrške za MSAL, čime će se osigurati da će imati koristi u trajnoj sigurnosti i poboljšanjima značajki koje je mala.

1. [Pročitajte najčešća pitanja o dodatku](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Saznajte kako migrirati aplikacije na osnovi po platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Ako nakon čitanja vodiča za platformu aplikacije imate dodatna pitanja, možete objavljivati na servisu [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) pomoću oznake [Azure-ad-Adal-depretcation] ili otvoriti problem u spremištu za GitHub biblioteke. Pogledajte odjeljak [Jezici i okviri](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) u članku **Pregled msal** -a za veze na repo svake biblioteke.
4. **Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL**, preporučujemo da pregledate izvorni kod svih aplikacija. Ako je primjenjivo, obratite se svim neovisnim dobavljačima softvera (ISVs) ili pružateljima aplikacija. Microsoftova podrška također vam može pružiti popis svih aplikacija koje nisu Microsoftove ADAL u vašem klijentu.







