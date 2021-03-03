---
title: Uklanjanje podataka i brisanje uređaja iz programa Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416305"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Uklanjanje podataka i brisanje uređaja iz programa Intune

Uređaj se povlači, a uređaj briše udaljene akcije, može se koristiti za uklanjanje podataka tvrtke koje upravlja Intune ili za izvođenje tvornice i vraćanje uređaja na zadane postavke.

1. Prijavite se u upravljanje uređajima Microsoft 365, a zatim otvorite **Uređaji**  >  **Svi uređaji**.
2. Odaberite uređaj koji želite izbrisati.
3. Odaberite vrstu daljinskog brisanja koju želite učiniti. Povlačenje briše samo organizacijske podatke, dok pune maramice vraćaju uređaj na tvorničke postavke.
4. Odaberite **da** da biste potvrdili. Dok brisanje ne završi, status akcije uređaja prikazuje se kao *umirovljen na čekanju*.
    Nakon dovršetka akcije više nećete vidjeti mobilni uređaj na popisu upravljanog uređaja.

> [!NOTE]
> Podaci o poduzeću ne mogu se ukloniti s uređaja koji su spojeni na Azure AD. 

Informacije o efektu umirovljenja i brisanja, uključujući ono što je sačuvano i izbrisano, potražite u članku sljedeća dokumentacija:

- [Uklonite uređaje pomoću značajke brisanje, povlačenje ili ručno poništavanje upisivanjem uređaja](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Brisanje samo korporativnih podataka iz aplikacija koje upravlja Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Brisanje svih podataka s macOS uređaja](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).