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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583240"
---
# <a name="rbac-rules"></a>RBAC pravila

Ako vam se prikaže pogreška s dozvolom: 

- **Naručitelj s ID-om objekta nema ovlaštenje za izvršavanje akcije nad optikom (kod: Autorizacija nije ispunilo proročanstvo)**: kada pokušate stvoriti resurs, provjerite jeste li trenutno prijavljeni uz korisnika kojem je dodijeljena uloga koja sadrži dozvolu za zapisivanje resursa u odabranom opsegu. Da biste, primjerice, upravljali virtualnim strojevima u grupi resursa, trebali biste imati ulogu [suradnika virtualnog stroja](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) u grupi resursa (ili nadređenom opsegu). Popis dozvola za svaku ugrađenu ulogu potražite [u članku ugrađene uloge za resurse Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- Nemate **dozvolu za stvaranje zahtjeva za podršku**: kada pokušate stvoriti ili ažurirati ulaznicu za podršku, provjerite jeste li trenutno prijavljeni uz korisnika kojem je dodijeljena uloga koja sadrži dozvolu Microsoft. support/supportTickets/Write, kao što je [suradnik zahtjeva za podršku](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Nema više dodjela uloga koje je moguće stvoriti (kod: Roledodjela vrijednosti)**: kada pokušate dodijeliti ulogu, pokušajte smanjiti broj dodjela uloga tako da dodijelite uloge grupama. Azure podržava do **2000** dodjela uloga po pretplati.

Dodatne informacije o ulogama Azure RBAC potražite u članku [Azure RBAC uloge](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
