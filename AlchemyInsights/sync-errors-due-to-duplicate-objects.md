---
title: 902 (pogreške pri sinkronizaciji zbog dupliciranih objekata)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708054"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Pogreške prilikom sinkronizacije zbog dupliciranih objekata

Možda će vam se prikazati jedna od sljedećih poruka o pogrešci kada sinkronizacija direktorija završi u programu Microsoft 365:

- Nije moguće ažurirati ovaj objekt u Microsoftovim internetskim servisima jer sljedeći atributi pridruženi ovom objektu imaju vrijednosti koje su možda već povezane s drugim objektom u lokalnom direktoriju.

- Sinkronizirani objekt s istom proxy adresom već postoji u direktoriju Microsoftova internetskih servisa.

- Ovaj objekt nije moguće ažurirati jer sljedeći atributi pridruženi ovom objektu imaju vrijednosti koje se možda već povezuju s drugim objektom u lokalnim imeničkim servisima: UserPrincipalName.

Da biste identificirali i riješili problem, Preuzmite i pokrenite [alat za ispravljanje pogrešaka u Idfix DirSync](https://github.com/Microsoft/idfix).

Dodatne informacije potražite u članku [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
