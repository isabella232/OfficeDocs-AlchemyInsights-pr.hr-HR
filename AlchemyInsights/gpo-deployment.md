---
title: Implementacija GPO-a
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427015"
---
# <a name="gpo-deployment"></a>Implementacija GPO-a

Postavke za korisničke i računalne objekte u servisu Azure Active Directory domene (Azure AD DS) često se upravljaju pomoću objekata pravilnika grupe (GPOs-a). Azure AD DS sadrži ugrađene GPOs-ove za korisnike AADDC i kontejnere AADDC Computers. Te ugrađene GPOs možete prilagoditi za konfiguriranje pravilnika grupe prema potrebi za okruženje. Članovi grupe Administratori Azure AD DC imaju privilegije za administraciju pravilnika grupe u domeni Azure AD DS, a mogu stvarati i prilagođene GPOs i organizacijske jedinice (OUs). Dodatne informacije o pravilima grupe i načinu rada potražite u članku [Pregled pravilnika grupe](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

U hibridnom okruženju pravila grupe konfigurirana u lokalnom okruženju AD DS nisu sinkronizirane sa servisom Azure AD DS. Da biste definirali konfiguracijske postavke za korisnike ili računala u servisu Azure AD DS, uredite jedan od zadanih GPOs-a ili stvorite prilagođeni GPO.

U ovom se članku [upravlja pravilima grupe](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) , a prikazuje se kako instalirati alate za upravljanje pravilima grupe, kako ton uređivati ugrađene gpos-ove i kako stvoriti prilagođene gpos-ove.
