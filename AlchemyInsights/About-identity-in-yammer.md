---
title: O identitetu na servisa Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148179"
---
# <a name="about-identity-in-yammer"></a>O identitetu na servisa Yammer

Preporučuje se da sve mreže poduzmu sljedeće korake kako bi izbjegle probleme povezane s identitetom:

1. Nametni identitet sustava Office 365 nakon dodjele računa sustava Microsoft 365 za korisnike u azure AD da biste bili sigurni da se svi korisnici prijavljuju pomoću primarnog računa za Microsoft 365. Dodatne informacije potražite u članku [Nametanje identiteta sustava Office 365 za korisnike servisa Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidirajte više mreža servisa Yammer. Naslijeđene konfiguracije servisa Yammer omogućuju povezivanje više mreža servisa Yammer s jednim klijentom. Dodatne informacije potražite u [odjeljku Migracija mreže – konsolidacija više mreža servisa Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Po želji, nametni licenciranje za Yammer da blokira korisnike sa servisa Yammer ako nemaju licencu. Dodatne informacije [potražite u odjeljku Upravljanje korisničkim licencama servisa Yammer u sustavu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Konačno, pregledajte popis korisnika za starije mreže servisa Yammer i obustavite naslijeđenu korisnike. Preporučuje se da obustavite (deaktivirati) korisnike umjesto da ih izbrišete jer je brisanje nepovratno. Dodatne informacije potražite [u odjeljku Nadzor korisnika servisa Yammer u mrežama povezanima sa sustavom Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) i [Uklanjanje korisnika](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Konfiguriranjem servisa Yammer pomoću ovih koraka bit ćete spremni konfigurirati mrežu servisa Yammer za izvorni način rada za Microsoft 365. Dodatne informacije [potražite u odjeljku Konfiguriranje mreže servisa Yammer za izvorni način rada za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).