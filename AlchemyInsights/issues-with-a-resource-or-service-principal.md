---
title: Problemi s resursom ili upraviteljem servisa
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028068"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemi s resursom ili upraviteljem servisa

1. Ako tek počinjete s radom, glavni objekti aplikacije i servisa [u programu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) opisuju registraciju aplikacije, objekte aplikacija i upravitelje servisa u aplikaciji Azure Active Directory: što su oni, kako se koriste i kako su međusobno povezani. Prikazuje se i scenarij s više klijenta koji ilustrira odnos između objekta aplikacije i odgovarajućih glavnih objekata servisa.
2. Dodatne informacije o odnosu između aplikacija i upravitelja servisa možete saznati čitanjem aplikacija [i glavnih objekata servisa u Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Upute: pomoću portala](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) stvorite aplikaciju Azure AD i upravitelja servisa koji mogu pristupiti resursima pokazuje kako stvoriti novu aplikaciju Azure Active Directory (Azure AD) i upravitelja servisa koji se mogu koristiti s kontrolom pristupa utemeljenom na ulogama.
4. Uz [glavni API servisa](https://docs.microsoft.com/graph/api/resources/serviceprincipal)možete programski upravljati instancama aplikacija i kontrolirati što aplikacija može učiniti unutar klijenta.
5. [servicePrincipal resource type lists](https://docs.microsoft.com/graph/api/resources/serviceprincipal) all properties and methods for the servicePrincipal resource type.
6. [Razlike u vrsti resursa između servisa Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) ističe razlike između resursa servisa Azure AD Graph i Microsoft Graph. Prikazuje resurse koji imaju različite nazive ili nisu dostupni; ujedno ističe resurse dostupne u beta verziji programa Microsoft Graph, ali ne i u verziji v1.0.

**Problemi s gostima**

- [Brzi početak rada:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) dodavanje gostiju u direktorij na portalu Azure pokazuje kako dodati novog gosta u direktorij servisa Azure AD putem portala Azure, poslati pozivnicu i vidjeti kako izgleda postupak otkupa pozivnice gosta.
- [Vodič: stvaranje korisničkih tokova u Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) pokazuje kako stvoriti neke preporučene korisničke tokove pomoću portala Azure. Ako tražite informacije o tome kako postaviti tijek vjerodajnica za lozinku vlasnika resursa (ROPC) u aplikaciji, pogledajte konfiguriranje tijeka vjerodajnica za lozinku vlasnika resursa na servisu Azure AD B2C.
