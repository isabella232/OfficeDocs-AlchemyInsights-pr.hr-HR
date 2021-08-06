---
title: Upit o API-ju Graph microsofta
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923231"
---
# <a name="querying-the-microsoft-graph-api"></a>Upit o API-ju Graph microsofta

Ova se tema može primijeniti i na razvojne inženjere koji i dalje koriste AZURE AD Graph API. No preporučuje se **da koristite** Microsoft Graph za sve scenarije direktorija, identiteta i upravljanja pristupom.

**Problemi s provjerom autentičnosti ili autorizacijom**

- Ako vaša aplikacija ne može nabaviti **tokene** da bi zvala Microsoft Graph, odaberite Problem s dohvaćanje tokena za **pristup (provjera autentičnosti)** Microsoft Graph kategorije da biste dobili konkretnu pomoć i podršku za ovu temu.
- Ako aplikacija prima **401 ili 403** pogreške u autorizaciji prilikom pozivanja microsofta Graph, odaberite kategoriju Dobivanje pogreške o odbijenom **pristupu (Autorizacija)** microsoft Graph API kategorije da biste dobili konkretnu pomoć i podršku za ovu temu.

**Želim koristiti Microsoft Graph, ali ne znam gdje početi**

Dodatne informacije o programu Microsoft Graph potražite u članku:

- [Pregled programa Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled upravljanja identitetom i pristupom u programu Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Početak rada s radom u aplikacijama Graph Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – testirajte API-je Graph Microsofta na klijentu ili na oglednom klijentu

**Želim koristiti Microsoft Graph, ali podržava li apije direktorija v1.0 koje su mi potrebne?**

Microsoft Graph preporučeni API za upravljanje direktorijem, identitetom i pristupom. No i dalje postoji nekoliko praznina između mogućnosti servisa Azure AD Graph Microsoft Graph. Pregledajte sljedeće članke u kojima se ističu najatragnije razlike koje će vam pomoći u odabiru:

- [Razlike u vrsti resursa između servisa Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike u svojstva između servisa Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Razlike u metodi između servisa Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Kada upitam objekt *korisnika,* nedostaju mnoga njegova svojstva**

`GET https://graph.microsoft.com/v1.0/users`vraća samo 11 svojstava jer Microsoft Graph automatski odabire zadani skup *korisničkih svojstava za* vraćanje. Ako su vam potrebna *druga korisnička* svojstva, pomoću $select odaberite svojstva koja su potrebna vašoj aplikaciji. Najprije isprobajte u **programu Microsoft Graph Explorer.**

**Neke vrijednosti svojste korisnika *imaju vrijednost null* iako znam da su postavljene**

Najvjerojatnije je objašnjenje da je aplikaciji dodijeljena dozvola *User.ReadBasic.All.* To aplikaciji omogućuje čitanje ograničenog skupa korisničkih svojstava, vraćanje svih ostalih svojstava kao null čak i ako su prethodno postavljena. Pokušajte umjesto toga dodjeljujte *aplikaciju User.Read.All* dozvolu.

Dodatne informacije potražite u članku [Korisničke Graph microsofta](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Imam problema s korištenjem OData parametara upita za filtriranje podataka u svojim zahtjevima**

Iako Microsoft Graph podržava širok raspon parametara OData upita, mnoge od tih parametara ne podržavaju u potpunosti imenički servisi (resursi koji nasljeđuju od *direktorijaObject*) u programu Microsoft Graph. Ista ograničenja koja su bila prisutna u servisu Azure AD Graph uglavnom se zadržavaju u programu Microsoft Graph:

1. **Nije podržano**: $count, $search i $filter *vrijednosti* null ili *ne*
2. **Nije podržano**: $filter određenih svojstava (pogledajte teme resursa o tome koja se svojstva mogu filtrirati)
3. **Nije podržano:** istodobno straničenje, filtriranje i sortiranje
4. **Nije podržano:** filtriranje odnosa. Na primjer – pronađite sve članove inženjerske grupe koji se nalaze u Velikoj Britaniji.
5. **Djelomična podrška**: $orderby *korisniku* (samo displayName i userPrincipalName) i *grupi*
6. **Djelomična** podrška : $filter (podržava samo *eq*, *počinje* s podrškom *ili* *,* i , i ograničenom ) podrškom, $expand (proširivanje odnosa jednog objekta vraća sve odnose, ali proširivanje zbirke odnosa objekata je ograničeno)

Dodatne informacije potražite u članku [Prilagodba odgovora parametrima upita](https://docs.microsoft.com/graph/query-parameters).

**API koji pozivam ne funkcionira – gdje mogu učiniti više testiranja?**

**Microsoft Graph Explorer** – testirajte API-je microsoft Graph na klijentu ili oglednom klijentu te pogledajte ogledne upite **u** programu Microsoft Graph Explorer.

**Prilikom upita za podatke čini se da mi se vraća nepotpun skup podataka**

Ako upitujete zbirku (kao što su *korisnici),* Microsoft Graph koristi ograničenja stranica na strani poslužitelja da bi se rezultati uvijek vraćali sa zadanom veličinom stranice. Vaša bi aplikacija uvijek trebala očekivati da će se stranica preusmjehivati putem zbirki koje se vraćaju iz servisa.

Dodatne informacije potražite u sljedećim člancima:

- [Najbolje prakse Graph microsofta](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging Microsoft Graph podataka u aplikaciji](https://docs.microsoft.com/graph/paging)

**Aplikacija je prespora i usporava se. Koja poboljšanja mogu učiniti?**

Ovisno o scenariju, na raspolaganju su vam brojne različite mogućnosti da bi aplikacija bila performantna, a u nekim slučajevima manje sklona tome da vas servis gasi (kada upućivanje previše poziva).

Dodatne informacije potražite u člancima:

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
