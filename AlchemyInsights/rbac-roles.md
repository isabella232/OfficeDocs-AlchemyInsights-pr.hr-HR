---
title: 'RBAC uloge '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923123"
---
# <a name="rbac-rules"></a>RBAC pravila

Ako vam se pojavi pogreška s dozvolama: 

- Klijent s ID-om objekta nema ovlaštenje za izvršavanje akcije preko opsega **(kod: AuthorizationFailed):** kada pokušate stvoriti resurs, provjerite jeste li trenutno prijavljeni s korisnikom koji ima ulogu koja ima dozvolu za pisanje resursa u odabranom opsegu. Da biste, primjerice, upravljali virtualnim računalima u grupi resursa, trebali biste imati ulogu suradničku ulogu virtualnog računala u grupi resursa (ili nadređenom opsegu). [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) Popis dozvola za svaku ugrađenu ulogu potražite u članku Ugrađene [uloge za resurse sustava Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Nemate dozvolu** za stvaranje zahtjeva za podršku : kada pokušate stvoriti ili ažurirati kartu za podršku, provjerite jeste li trenutno prijavljeni s korisnikom koji ima ulogu koja ima dozvolu Microsoft.Support/supportTickets/write, kao što je suradnik zahtjeva [za podršku](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- Nije moguće stvarati više zadataka **uloga (kod: RoleAssignmentLimitExceeded):** kada pokušate dodijeliti ulogu, pokušajte smanjiti broj zadataka uloga dodjelom uloga grupama. Azure podržava do **2000** zadataka uloga po pretplati.

Dodatne informacije o ulogama za Azure RBAC potražite u članku [Uloge za Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
