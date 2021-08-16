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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067832"
---
# <a name="gpo-deployment"></a>Implementacija GPO-a

Postavke za korisničke i računalne objekte u servisu Azure Active Directory Domain Services (Azure AD DS) često se upravlja pomoću objekata pravilnika grupe (GPO-ove). Azure AD DS sadrži ugrađene GPO-ove za AADDC korisnike i spremnike AADDC računala. Te ugrađene GPO-ove možete prilagoditi tako da konfiguriraju pravilnik grupe prema potrebi za svoje okruženje. Članovi grupe administratora servisa Azure AD DC imaju ovlasti administracije pravilnika grupe u domeni Azure AD DS, a mogu i stvarati prilagođene GPO-ove i organizacijske jedinice (OU-ove). Dodatne informacije o pravilniku grupe i kako to funkcionira potražite u članku [Pregled pravilnika grupe](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

U hibridnom okruženju pravilnike grupe konfigurirane u lokalnom okruženju AD DS ne sinkroniziraju se sa servisom Azure AD DS. Da biste definirali postavke konfiguracije za korisnike ili računala na servisu Azure AD DS, uredite jedan od zadanih GPO-ova ili stvorite prilagođeni GPO.

Ovaj članak [Upravljanje pravilnikom](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) grupe pokazuje kako instalirati alate za upravljanje pravilnikom grupe, kako ton uređivati ugrađene GPO-ove i kako stvoriti prilagođene GPO-ove.
