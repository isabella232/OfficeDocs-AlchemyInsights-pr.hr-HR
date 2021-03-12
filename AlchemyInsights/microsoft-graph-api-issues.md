---
title: Problemi s API-jem u programu Microsoft Graph
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713472"
---
# <a name="microsoft-graph-api-issues"></a>Problemi s API-jem u programu Microsoft Graph

Ova se tema može primijeniti i na programere koji se i dalje koriste API-jem Azure AD Graph. Međutim **, preporuča se** da koristite Microsoft Graph za sve vaše mape, identitete i upravljanje pristupom.

**Problemi s autentifikaciju i autorizacija**

- Ako aplikacija **ne može nabaviti tokene** za pozivanje programa Microsoft Graph, odaberite **problem s mogućnošću dobivanja tokena programa Access (provjera autentičnosti)** u kategoriji Microsoft Graph da biste dobili konkretniju pomoć i podršku u ovoj temi.
- Ako aplikacija **dobiva 401 ili 403 pogreške** prilikom pozivanja programa Microsoft Graph, odaberite kategoriju **Dohvaćanje pogreške (autorizacija)** sustava Microsoft Graph API da biste dobili konkretniju pomoć i podršku u ovoj temi.

**Želim koristiti Microsoft Graph, ali ne znam gdje početi**

- [Pregled programa Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled identiteta i upravljanja pristupom u programu Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Početak izgradnje aplikacija Microsoft Graph](https://docs.microsoft.com/graph/)
- **Eksplorer za Microsoft Graph** – testiranje programa Microsoft Graph u klijentu ili demo klijentu

**Želim koristiti Microsoft Graph, ali podržava li API-ju direktorija v 1.0 koji mi je potreban?**

Microsoft Graph Preporučeni je API za upravljanje direktoriju, Identity i Access. No još ima nekoliko praznina između mogućnosti u programu Azure AD Graph i Microsoft Graph. Pregledajte sljedeće članke, što naglašava najnovije razlike koje će vam pomoći u odabiru:

- [Razlike u vrsti resursa između Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike u svojstvima između Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Metode razlike između servisa Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API koji pozivam ne funkcionira – gdje se mogu dodatno testirati?**

**Eksplorer za Microsoft Graph** -Testirajte Microsoft Graph Apis u klijentu ili demo klijentu, a pogledajte i **ogledne upite** u programu Microsoft Graph Explorer.

**Moja aplikacija je prespora, a dobiva se i grlo. Koja poboljšanja mogu unijeti?**

Ovisno o scenariju, na raspolaganju su vam razne mogućnosti da bi vaša aplikacija bila više performant, a u nekim slučajevima i manje skloni tome da ga servis upravlja (kada ste učinili previše poziva).

- [Najbolja praksa u programu Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Zahtjevi za bating](https://docs.microsoft.com/graph/json-batching)
- [Evidentiranje promjena putem Delta upita](https://docs.microsoft.com/graph/delta-query-overview)
- [Primanje obavijesti o promjenama putem webkuke](https://docs.microsoft.com/graph/webhooks)
- [Smjernice za ograničavanje](https://docs.microsoft.com/graph/throttling)

**Gdje mogu pronaći dodatne informacije o pogreškama i poznatim problemima?**

- [Podaci o pogrešci odgovora na Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Poznati problemi s programom Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Gdje mogu provjeriti status dostupnosti i povezivanja servisa?**

Dostupnost servisa i povezivanje osnovnih servisa kojima se može pristupiti putem programa Microsoft Graph može utjecati na ukupnu dostupnost i performanse programa Microsoft Graph.

- Da biste provjerili stanje servisa Azure Active Directory, provjerite status **sigurnosnih + identifikacijskih** servisa navedenih na [stranici statusa Azure](https://azure.microsoft.com/status/).
- Za servise sustava Office koji pridonose programu Microsoft Graph provjerite status servisa navedenih na [nadzornoj ploči zdravstvene službe sustava Office](https://portal.office.com/adminportal/home#/servicehealth).

Pogreške autorizacije u programu Microsoft Graph mogu biti rezultat nekoliko različitih problema, od kojih većina generira pogrešku 401 ili 403. Na primjer, sljedeće može dovesti do pogrešaka autorizacije:

- Netočni [tijekovi prikupljanja pristupnog tokena](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Loše konfigurirani [opsezi dopuštenja](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Kraj podrške za Azure Active Directory Authentication Library (ADAL) i Azure AD Graph API (AAD Graph)_* _

_ * Počevši od 30 Lipanj, 2020 * *, više nećemo dodavati nove značajke u ADAL i Azure AD Graph. I dalje ćemo pružati tehničku podršku i sigurnosna ažuriranja, ali više nećemo pružati ažuriranja značajki.

**Počevši od 30 lipnja 2022**, završit ćemo podršku za Adal i Azure ad Graph i više neće pružati tehničku podršku ni Sigurnosno ažuriranje.

Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće *dobiti nikakvu tehničku podršku ni Sigurnosno ažuriranje*.

Aplikacije koje koriste Azure AD Graph nakon tog vremena možda više neće primati odgovore iz krajnjih točaka Azure AD Graph.

**ADAL migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) koja ima najnovije značajke i sigurnosna ažuriranja.

Ako koristite Microsoftove aplikacije, znajte da je Microsoft u postupku migracije svojih aplikacija u MSAL uz krajnji rok za potporu, čime će se osigurati da koristi MSAL-ove trajne sigurnosti i poboljšanja značajki.

1. [Pročitajte najčešća pitanja vezana za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saznajte kako migrirati aplikacije na platformu](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL, preporučujemo vam da pregledate sve izvorne šifre aplikacija i ako je primjenjivo, obratite se svim pružateljima programa ISVs ili aplikacije. Microsoftova podrška također vam može pružiti popis svih aplikacija koje nisu Microsoftove ADAL u vašem klijentu.

**Migracija grafikona AAD**

Za aplikacije koje koriste Azure AD Graph, slijedite upute da biste [migrirali aplikacije Azure ad Graph u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Naš popis za migraciju pruža točku početka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Vaš portal za registraciju Azure aplikacija prikazuje koje aplikacije koriste AAD Graph. Preporučujemo da pregledate izvorni kod svih aplikacija i ako je primjenjivo obratite se svim ISV-ovima ili davateljima aplikacija. Microsoftova podrška može vam pružiti i popis svih korištenja AAD grafikona u vašem zakupcu.
3. Da bi aplikacija pristupio podacima u programu Microsoft Graph, korisnik ili administrator mora mu dodijeliti ispravne dozvole putem postupka pristanka. [Referenca dozvola za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) prikazuje popise dozvola povezanih sa svakim glavnim skupom programa Microsoft Graph Apis. Nudi i upute za korištenje dozvola.
