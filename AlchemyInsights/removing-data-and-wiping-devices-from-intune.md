---
title: Uklanjanje podataka i brisanje uređaja iz intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438913"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Uklanjanje podataka i brisanje uređaja iz intune

Daljinske akcije za povlačenje uređaja i brisanje uređaja mogu se koristiti za uklanjanje podataka tvrtke kojima upravlja Intune ili za vraćanje na tvorničke postavke i vraćanje uređaja na zadane postavke.

1. Prijavite se u Microsoft 365 Device Management i idite na **Uređaji**  >  **svi uređaji**.
2. Odaberite uređaj koji želite izbrisati.
3. Odaberite vrstu daljinskog brisanja koju želite učiniti. Povlačenjem se brišu samo organizacijske informacije, dok potpuno brisanje vraća uređaj na tvorničke postavke.
4. Odaberite **Da** za potvrdu. Dok brisanje ne završi, status akcije Uređaja prikazuje se kao Neriješeno.</br>
    Nakon dovršetka akcije mobilni uređaj više nećete vidjeti na popisu upravljanih uređaja.

**Napomena:** Podaci tvrtke ne mogu se ukloniti s uređaja pridruženih azure AD.

Potpune pojedinosti o učinku akcija "Umirovljenje i brisanje" u svrhu povlačenja i brisanja potražite u [odjeljku Uklanjanje uređaja brisanjem, povlačenjem ili ručnim uklanjanjem uređaja](https://docs.microsoft.com/intune/devices-wipe).

Da biste izbrisali sve podatke s macOS uređaja, pročitajte pravila [Brisanje svih podataka s macOS uređaja](https://docs.microsoft.com/intune/device-erase).