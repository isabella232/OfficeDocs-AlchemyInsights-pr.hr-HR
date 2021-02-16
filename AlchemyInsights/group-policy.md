---
title: Pravilnik grupe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256666"
---
# <a name="group-policy"></a>Pravilnik grupe

Postavke za korisničke i računalne objekte u servisu Azure Active Directory domene (Azure AD DS) često se upravljaju pomoću objekata pravilnika grupe (GPOs-a). Azure AD DS sadrži ugrađene GPOs-ove za korisnike AADDC i kontejnere AADDC Computers. Te ugrađene GPOs možete prilagoditi za konfiguriranje pravilnika grupe prema potrebi za okruženje. Članovi grupe Administratori Azure AD DC imaju privilegije za administraciju pravilnika grupe u domeni Azure AD DS, a mogu stvarati i prilagođene GPOs i organizacijske jedinice (OUs). Dodatne informacije o pravilima grupe i načinu rada potražite u članku [Pregled pravilnika grupe](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

U hibridnom okruženju pravila grupe konfigurirana u lokalnom okruženju AD DS nisu sinkronizirane sa servisom Azure AD DS. Da biste definirali konfiguracijske postavke za korisnike ili računala u servisu Azure AD DS, uredite jedan od zadanih GPOs-a ili stvorite prilagođeni GPO.

U ovom se članku [upravlja pravilima grupe](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) , a prikazuje se kako instalirati alate za upravljanje pravilima grupe, kako ton uređivati ugrađene gpos-ove i kako stvoriti prilagođene gpos-ove.



