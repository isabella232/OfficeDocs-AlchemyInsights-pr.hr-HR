---
title: Problemi s resursom ili upraviteljicom servisa
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
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50713448"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemi s resursom ili upraviteljicom servisa

1. Ako ste tek početak rada, [osnovni objekti aplikacija i servisa u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) opisuju registraciju aplikacija, objekte aplikacija i ravnatelje servisa u servisu Azure Active Directory: ono što jesu, način na koji se koriste i kako se međusobno odnose. Prikazuje se i ogledni scenario s više klijenata da bi se ilustrirao odnos između objekta aplikacija i odgovarajućih osnovnih objekata servisa.
2. Dodatne informacije o odnosima između aplikacija i ravnatelja servisa možete pronaći čitanjem [aplikacija i osnovnih objekata u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Kako: pomoću portala stvoriti aplikaciju Azure ad i upravitelj servisa koji omogućuje pristup resursima](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) prikazuje kako stvoriti novu aplikaciju Azure Active Directory (Azure AD) i upravitelja servisa koja se može koristiti u kontroli pristupa utemeljenoj na ulozi.
4. Pomoću glavnog [API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)-ja za servis možete programsko upravljati instancama aplikacija i kontrolirati što aplikacija može učiniti u vašem zakupcu.
5. [Vrsta resursa serviceprincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) navodi sva svojstva i metode za grupu resursa servisa serviceprincipal.
6. [Razlike u vrsti resursa između Azure ad Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) ističe razlike između Azure ad Graph i Microsoft Graph resursa. Prikazat će se resursi koji imaju različita imena ili nisu dostupni; Ona također ističe resurse dostupne u beta verziji programa Microsoft Graph, ali ne i u verziji v 1,0.

**Problemi s korisnicima gostiju**

- Brzi [početak rada: Dodavanje korisnika u direktorij na portalu Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) prikazuje kako dodati novog gosta u direktorij Azure ad putem portala Azure, poslat ćete pozivnicu i vidjeti kako izgleda postupak otkupa pozivnice za gosta.
- [Udžbenik: Stvaranje korisničkih tokova u servisu Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) prikazuje kako stvoriti neki Preporučeni korisnički protok pomoću portala Azure. Ako tražite informacije o tome kako odrediti tijek vjerodajnica za lozinku vlasnika resursa (ROPC) u aplikaciji, pročitajte članak konfiguriranje tijeka vjerodajnica za lozinku vlasnika resursa u servisu Azure AD B2C.
