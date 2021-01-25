---
title: Mapiranje atributa korisnika-dodjela resursa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949665"
---
# <a name="user-provisioning-attribute-mapping"></a>Mapiranje atributa korisnika-dodjela resursa

1. Da biste otklonili poteškoće s poznatim problemima s preslikavanjem atributa, pogledajte [preslikavanje atributa](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) nudi podršku za dodjelu resursa korisnicima u programu SaaS kao što su Salesforce, G suite i drugi. Ako korisnicima omogućite dodjelu resursa za aplikaciju za SaaS, portal Azure upravlja vrijednostima atributa pomoću mapiranja atributa. Upute za prilagodbu zadanog mapiranja atributa potražite [u članku Prilagodba atributa korisničke dodjele resursa – mapiranja za aplikacije SaaS u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Da biste saznali više o dodjeli resursa korisnika u aplikaciji SaaS, pročitajte članak [što je automatska dodjela korisničkih aplikacija za SaaS u Azure ad?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Prilikom prilagodbe atributa – mapiranja za dodjelu resursa korisniku, možda ćete pronaći da se atribut koji želite mapirati ne prikazuje na popisu izvorišni atribut. [Sinkroniziranje atributa iz lokalnog servisa Active Directory sa servisom Azure ad za dodjelu resursa u članak aplikacije](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) prikazuje kako dodati atribut koji nema sinkroniziranjem s lokalnog oglasa na Azure AD.
