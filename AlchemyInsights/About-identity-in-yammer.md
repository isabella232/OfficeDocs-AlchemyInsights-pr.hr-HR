---
title: O identitetu u Yammer
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
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918929"
---
# <a name="about-identity-in-yammer"></a>O identitetu u Yammer

Preporučuje se da sve mreže poduzmu sljedeće korake da bi se izbjegli problemi povezani s identitetom:

1. Nametanje Office 365 identiteta nakon dodjele resursa Microsoft 365 za korisnike na servisu Azure AD da bi se svi korisnici prijavili pomoću primarnog Microsoft 365 računa. Dodatne informacije potražite u članku [Nametanje Office 365 identiteta Yammer korisnicima](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidirajte više Yammer mreža. Naslijeđene Yammer omogućuju povezivanje više Yammer s jednim klijentom. Dodatne informacije potražite u članku [Migracija mreže – konsolidacija većeg broja Yammer mreža](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Ako želite, nametnuti licenciranje Yammer da biste korisnicima blokirali Yammer ako nemaju licencu. Dodatne informacije potražite u članku [Upravljanje korisničkim Yammer licencama u sustavu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Naposljetku, nadziranje popisa korisnika za starije Yammer i obustavljanje naslijeđenih korisnika. Preporučuje se obustaviti (deaktivirati) korisnike umjesto da ih izbrišete jer je brisanje nepovratno. Dodatne informacije potražite u članku Nadzor [Yammer korisnicima u mrežama povezanima s Office 365 i Uklanjanje](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) [korisnika](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Konfiguriranjem Yammer sljedećih koraka bit ćete spremni i konfigurirati mrežu Yammer za nativni način rada za Microsoft 365. Dodatne informacije potražite u članku [Konfiguriranje mreže Yammer za nativni način rada za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).