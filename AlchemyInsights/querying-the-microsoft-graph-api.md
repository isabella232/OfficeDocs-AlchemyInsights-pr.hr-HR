---
title: Postavljanje upita u API-ju programa Microsoft Graph
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974215"
---
# <a name="querying-the-microsoft-graph-api"></a>Postavljanje upita u API-ju programa Microsoft Graph

Ova se tema može primijeniti i na programere koji se i dalje koriste API-jem Azure AD Graph. Međutim **, preporuča se** da koristite Microsoft Graph za sve vaše mape, identitete i upravljanje pristupom.

**Problemi s autentifikaciju i autorizacija**

- Ako aplikacija **ne može nabaviti tokene** za pozivanje programa Microsoft Graph, odaberite **problem s mogućnošću dobivanja tokena programa Access (provjera autentičnosti)** u kategoriji Microsoft Graph da biste dobili konkretniju pomoć i podršku u ovoj temi.
- Ako aplikacija **dobiva 401 ili 403 pogreške** prilikom pozivanja programa Microsoft Graph, odaberite kategoriju **Dohvaćanje pogreške (autorizacija)** sustava Microsoft Graph API da biste dobili konkretniju pomoć i podršku u ovoj temi.

**Želim koristiti Microsoft Graph, ali ne znam gdje početi**

Dodatne informacije o programu Microsoft Graph potražite u člancima:

- [Pregled programa Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled identiteta i upravljanja pristupom u programu Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Početak izgradnje aplikacija Microsoft Graph](https://docs.microsoft.com/graph/)
- **Eksplorer za Microsoft Graph** – testiranje programa Microsoft Graph u klijentu ili demo klijentu

**Želim koristiti Microsoft Graph, ali podržava li API-ju direktorija v 1.0 koji mi je potreban?**

Microsoft Graph Preporučeni je API za upravljanje direktoriju, Identity i Access. No još ima nekoliko praznina između mogućnosti u programu Azure AD Graph i Microsoft Graph. Pregledajte sljedeće članke, što naglašava najnovije razlike koje će vam pomoći u odabiru:

- [Razlike u vrsti resursa između Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike u svojstvima između Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Metode razlike između servisa Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Kada upitam *korisnički* objekt, nedostaju mnoga njegova svojstva**

`GET https://graph.microsoft.com/v1.0/users` vraća samo 11 svojstava, jer Microsoft Graph automatski odabire zadani skup *korisničkih* svojstava za povratak. Ako vam je potrebna druga *korisnička* svojstva, koristite $Select da biste odabrali svojstva koja je potrebna aplikaciji. Najprije isprobajte u programu **Microsoft Graph Explorer** .

**Neke su vrijednosti korisničkog svojstva *Null* iako znam da su postavljeni**

Najvjerojatnije je objašnjenje da je aplikaciji dodijeljen *korisnik. ReadBasic. sve* dozvole. Time se aplikaciji omogućuje čitanje ograničenog skupa korisničkih svojstava, vraćanje svih ostalih svojstava kao null, čak i ako su prethodno bili postavljeni. Pokušajte dodijelite korisniku aplikacije *. pročitajte. svi* dozvola umjesto.

Dodatne informacije potražite u [članku korisničke dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Imam problema s upotrebom parametara OData Query za filtriranje podataka u mojim zahtjevima**

Dok Microsoft Graph podržava širok raspon parametara OData upita, mnogi od tih parametara nisu u potpunosti podržani od strane imeničkih servisa (resursa koji nasljeđuju od *Directoryobject*) u programu Microsoft Graph. Ista ograničenja koja su bila prisutna u programu Azure AD Graph najviše su dio u programu Microsoft Graph:

1. **Nije podržano**: $count, $search i $filter na *Null* ili *Not null* vrijednosti
2. **Nije podržano**: $filter na određenim svojstvima (Pogledajte teme resursa na kojima je moguće filtrirati svojstva)
3. **Nije podržano**: straničenje, filtriranje i sortiranje u isto vrijeme
4. **Nije podržano**: filtriranje odnosa. Na primjer – Pronađite sve članove grupe za inženjerstvo u Velikoj Britaniji.
5. **Djelomična podrška**: $OrderBy na *korisniku* (samo DisplayName i UserPrincipalName) i *grupa*
6. **Djelomična podrška**: $filter (podržava samo *IQ*, *Startswith*, *or*, *and* i ograničenu *bilo koju*) podršku, $Expand (proširenje odnosa jednog objekta vraća sve odnose, ali je ograničena zbirka odnosa objekata)

Dodatne informacije potražite u članku [Prilagodba odgovora s parametrima upita](https://docs.microsoft.com/graph/query-parameters).

**API koji pozivam ne funkcionira – gdje mogu učiniti više testiranja?**

**Eksplorer za Microsoft Graph** -Testirajte Microsoft Graph Apis u klijentu ili demo klijentu, a pogledajte i **ogledne upite** u programu Microsoft Graph Explorer.

**Prilikom upita za podatke čini se kao da dobivam nepotpun skup podataka natrag**

Ako postavljate upit za zbirku (kao što su *korisnici*), Microsoft Graph koristi ograničenja stranice poslužitelja pa se rezultati uvijek vraćaju s zadanom veličinom stranice. Aplikacija bi uvijek trebala očekivati da će se na nju prikazivati zbirke vraćene iz servisa.

Dodatne informacije potražite u članku:

- [Najbolja praksa u programu Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Podaci o programu Microsoft Graph u aplikaciji](https://docs.microsoft.com/graph/paging)

**Moja aplikacija je prespora, a dobiva se i grlo. Koja poboljšanja mogu unijeti?**

Ovisno o scenariju, na raspolaganju su vam razne mogućnosti da bi vam aplikacija bila više performant, a u nekim slučajevima i manje sklona tome da vas servis upravlja (kada stvarate previše poziva).

Dodatne informacije potražite u člancima:

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
