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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701275"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Uklanjanje podataka i brisanje uređaja iz programa Intune

Uređaj se povlači, a uređaj briše udaljene akcije, može se koristiti za uklanjanje podataka tvrtke koje upravlja Intune ili za izvođenje tvornice i vraćanje uređaja na zadane postavke.

1. Prijavite se u upravljanje uređajima Microsoft 365, a zatim otvorite **Uređaji**  >  **Svi uređaji**.
2. Odaberite uređaj koji želite izbrisati.
3. Odaberite vrstu daljinskog brisanja koju želite učiniti. Povlačenje briše samo organizacijske podatke, dok pune maramice vraćaju uređaj na tvorničke postavke.
4. Odaberite **da** da biste potvrdili. Dok brisanje ne završi, status akcije uređaja prikazuje se kao umirovljen na čekanju.</br>
    Nakon dovršetka akcije više nećete vidjeti mobilni uređaj na popisu upravljanog uređaja.

**Notes** Podaci o poduzeću ne mogu se ukloniti s uređaja koji su spojeni na Azure AD.

Sve pojedinosti o efektu umirovljenja i brisanja akcije, uključujući ono što je sačuvano i izbrisane, potražite u članku [uklanjanje uređaja pomoću značajke brisanja, umirovljenja ili ručnog brisanja uređaja](https://docs.microsoft.com/intune/devices-wipe).

Da biste izbrisali sve podatke s macOS uređaja, pročitajte članak [Brisanje svih podataka s MacOS uređaja](https://docs.microsoft.com/intune/device-erase).