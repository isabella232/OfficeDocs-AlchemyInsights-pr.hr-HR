---
title: Problemi s API-jem Graph microsofta
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
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975885"
---
# <a name="microsoft-graph-api-issues"></a>Problemi s API-jem Graph microsofta

Ova se tema može primijeniti i na razvojne inženjere koji i dalje koriste AZURE AD Graph API. No preporučuje se **da koristite** Microsoft Graph za sve scenarije direktorija, identiteta i upravljanja pristupom.

**Problemi s provjerom autentičnosti ili autorizacijom**

- Ako vaša aplikacija ne može nabaviti **tokene** da bi zvala Microsoft Graph, odaberite Problem s dohvaćanje tokena za **pristup (provjera autentičnosti)** Microsoft Graph kategorije da biste dobili konkretnu pomoć i podršku za ovu temu.
- Ako aplikacija prima **401 ili 403** pogreške u autorizaciji prilikom pozivanja microsofta Graph, odaberite kategoriju Dobivanje pogreške o odbijenom **pristupu (Autorizacija)** microsoft Graph API kategorije da biste dobili konkretnu pomoć i podršku za ovu temu.

**Želim koristiti Microsoft Graph, ali ne znam gdje početi**

- [Pregled programa Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled upravljanja identitetom i pristupom u programu Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Početak rada s radom u aplikacijama Graph Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – testirajte API-je Graph Microsofta na klijentu ili na oglednom klijentu

**Želim koristiti Microsoft Graph, ali podržava li apije direktorija v1.0 koje su mi potrebne?**

Microsoft Graph preporučeni API za upravljanje direktorijem, identitetom i pristupom. No i dalje postoji nekoliko praznina između mogućnosti servisa Azure AD Graph Microsoft Graph. Pregledajte sljedeće članke u kojima se ističu najatragnije razlike koje će vam pomoći u odabiru:

- [Razlike u vrsti resursa između servisa Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike u svojstva između servisa Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Razlike u metodi između servisa Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API koji pozivam ne funkcionira – gdje mogu učiniti više testiranja?**

**Microsoft Graph Explorer** – testirajte API-je microsoft Graph na klijentu ili oglednom klijentu te pogledajte ogledne upite **u** programu Microsoft Graph Explorer.

**Aplikacija je prespora i usporava se. Koja poboljšanja mogu učiniti?**

Ovisno o scenariju, na raspolaganju su vam razne mogućnosti da bi aplikacija bila performantna, a u nekim je slučajevima manje sklona tome da vas servis gasi (kada upućivanje previše poziva).

- [Najbolje prakse Graph microsofta](https://docs.microsoft.com/graph/best-practices-concept)
- [Skupni zahtjevi](https://docs.microsoft.com/graph/json-batching)
- [Evidentiranje promjena kroz delta upit](https://docs.microsoft.com/graph/delta-query-overview)
- [Primaj obavijesti o promjenama putem webhooksa](https://docs.microsoft.com/graph/webhooks)
- [Smjernice za ograničavanje](https://docs.microsoft.com/graph/throttling)

**Gdje mogu pronaći dodatne informacije o pogreškama i poznatim problemima?**

- [Informacije o Graph pogreškama u programu Microsoft](https://docs.microsoft.com/graph/errors)
- [Poznati problemi s programom Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Gdje mogu provjeriti status dostupnosti i povezivosti servisa?**

Dostupnost servisa i povezivost temeljnih servisa kojima se može pristupiti putem servisa Microsoft Graph mogu utjecati na ukupnu dostupnost i performanse microsoftovih Graph.

- Da Azure Active Directory stanje servisa, provjerite status servisa **Sigurnost + Identitet** servisa navedenih na [stranici stanja servisa Azure](https://azure.microsoft.com/status/).
- Da Office servise koji pridonose sustavu Microsoft Graph, provjerite status servisa navedenih u nadzornoj [Office stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).

Pogreške Graph autorizacije za Microsoft mogu biti rezultat nekoliko različitih problema, od kojih većina generira pogrešku 401 ili 403. Sljedeće, primjerice, može dovesti do pogrešaka u autorizaciji:

- Netočni [tijekovi prikupljanja pristupnog tokena](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Loše konfigurirani [opsezi dopuštenja](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Kraj podrške za Azure Active Directory provjere autentičnosti (ADAL) i AZURE AD Graph API (AAD Graph)***

**Od 30. lipnja 2020.** više nećemo dodavati nove značajke u ADAL i Azure AD Graph. I dalje ćemo pružati tehničku podršku i sigurnosna ažuriranja, ali više nećemo pružati ažuriranja značajki.

**Od 30. lipnja 2022.** završit ćemo podršku za ADAL i Azure AD Graph i više nećemo pružati tehničku podršku ni sigurnosna ažuriranja.

Aplikacije koje koriste ADAL u postojećim verzijama operacijskog sustava i dalje će funkcionirati nakon tog vremena, ali neće dobiti *tehničku podršku ni sigurnosna ažuriranja*.

Aplikacije koje koriste Azure AD Graph nakon tog vremena možda više neće primati odgovore od krajnje točke servisa Azure AD Graph.

**ADAL migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) koja ima najnovije značajke i sigurnosna ažuriranja.

Ako koristite Microsoftove aplikacije, znaj da Microsoft u tijeku s migriranjem aplikacija u MSAL do krajnjeg roka podrške jamči da će imati koristi od trajnih poboljšanja sigurnosti i značajki MSAL-a.

1. [Pročitajte najčešća pitanja vezana za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saznajte kako migrirati aplikacije na platformu](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL, preporučujemo da pregledate izvorni kod svih aplikacija i, ako je primjenjivo, kontaktirate bilo kojeg DAVATELJa internetskih usluga ili davatelja aplikacija. Microsoftova podrška također vam može pružiti popis svih aplikacija koje nisu Microsoftove ADAL u vašem klijentu.

**Migracija grafikona AAD**

Za aplikacije koje koriste Azure AD Graph slijedite naše [smjernice za migriranje](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)aplikacija Azure AD Graph u Microsoft Graph .

1. [Naš popis za migraciju pruža točku početka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Vaš portal za registraciju Azure aplikacija prikazuje koje aplikacije koriste AAD Graph. Preporučujemo da pregledate izvorni kod svih aplikacija i ako je primjenjivo obratite se svim ISV-ovima ili davateljima aplikacija. Microsoftova podrška može vam pružiti i popis svih Graph AAD-a u klijentu.
3. Da bi vaša aplikacija pristupala podacima u aplikaciji Microsoft Graph, korisnik ili administrator moraju mu dodijeliti odgovarajuće dozvole putem postupka pristanka. Referenca [dozvola za Microsoft Graph sadrži](https://docs.microsoft.com/graph/permissions-reference) popis dozvola povezanih sa svakim glavnim skupom API-ja Graph Microsofta. Sadrži i smjernice za korištenje dozvola.
