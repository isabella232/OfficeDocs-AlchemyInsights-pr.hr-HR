---
title: 902 (pogreške prilikom sinkronizacije zbog dupliciranih objekata)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998774"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Pogreške prilikom sinkronizacije zbog dupliciranih objekata

Kada sinkronizacija direktorija završi u programu Microsoft 365, možda ćete primiti jednu od sljedećih Microsoft 365:

- Taj objekt nije moguće ažurirati u web-aplikaciji Microsoft Online Services jer sljedeći atributi pridruženi ovom objektu imaju vrijednosti koje su možda već povezane s drugim objektom u lokalnom direktoriju.

- Sinkronizirani objekt s istom proxy adresom već postoji u direktoriju servisa Microsoft Online Services.

- Taj objekt nije moguće ažurirati jer sljedeći atributi pridruženi ovom objektu imaju vrijednosti koje su možda već povezane s drugim objektom u lokalnim imeničkim servisima: UserPrincipalName.

Da biste prepoznali i riješili problem, preuzmite i pokrenite alat za ispravljanje [pogrešaka servisa IdFix DirSync](https://github.com/Microsoft/idfix).

Dodatne informacije potražite u članku [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
