---
title: 902 (Pogreške pri sinkronizaciji zbog dupliciranih objekata)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767109"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Pogreške pri sinkronizaciji zbog dupliciranih objekata

Možda ćete primiti jednu od sljedećih poruka o pogrešci kada sinkronizacija direktorija završi u sustavu Microsoft 365:

- Ovaj objekt nije moguće ažurirati u Microsoft Online Services jer sljedeći atributi pridruženi ovom objektu imaju vrijednosti koje su možda već povezane s drugim objektom u lokalnom direktoriju.

- Sinkronizirani objekt s istom proxy adresom već postoji u imeniku Microsoft Online Services.

- Nije moguće ažurirati ovaj objekt jer sljedeći atributi pridruženi ovom objektu imaju vrijednosti koje su možda već povezane s drugim objektom u lokalnim imenišnim servisima: UserPrincipalName.

To prepoznati i škripac ispostavljati, preuzimanje datoteka i trčanje [IdFix DirSync Greška Ispravljanje Alat](https://www.microsoft.com/download/details.aspx?id=36832).

Dodatne informacije potražite u članku [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
