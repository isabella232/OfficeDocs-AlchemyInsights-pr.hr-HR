---
title: O identitetu u servisu Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664162"
---
# <a name="about-identity-in-yammer"></a>O identitetu u servisu Yammer

Preporučuje se da sve mreže poduzmu sljedeće korake da bi izbjegli probleme vezane uz identitet:

1. Provedba identiteta sustava Office 365 nakon dodjele resursa Microsoftovim 365 računima za korisnike u programu Azure AD da biste osigurali da se svi korisnici prijave pomoću primarnog računa za Microsoft 365. Dodatne informacije potražite u članku [Provedba identiteta sustava Office 365 za korisnike servisa Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidirate više mreža servisa Yammer. Naslijeđene konfiguracije servisa Yammer dozvoljavaju povezivanje više mreža servisa Yammer s jednim zakupcem. Dodatne informacije potražite u članku [Mrežna migracija – konsolidiranje više mreža servisa Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Po želji možete nametnuti licenciranje za Yammer da biste blokirali korisnike iz servisa Yammer ako nemaju licencu. Dodatne informacije potražite u članku [Upravljanje korisničkim dozvolama za Yammer u sustavu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Konačno, revidirajte popis korisnika starijih mreža servisa Yammer i obustavite naslijeđene korisnike. Preporučuje se da obustavite (deaktivirajte) korisnike umjesto da ih izbrišete jer je brisanje nepovratno. Dodatne informacije potražite u članku [nadzor nad korisnicima servisa Yammer u mrežama povezanim sa sustavom Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) i [uklanjanjem korisnika](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Ako konfigurirate Yammer pomoću ovih koraka, bit ćete spremni i konfigurirati mrežu servisa Yammer za izvorni način rada za Microsoft 365. Dodatne informacije potražite u članku [Konfiguriranje mreže servisa Yammer za izvorni način rada za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).