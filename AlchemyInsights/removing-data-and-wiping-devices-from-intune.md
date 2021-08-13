---
title: Uklanjanje podataka i brisanje uređaja iz aplikacije Intune
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
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922199"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Uklanjanje podataka i brisanje uređaja iz aplikacije Intune

Daljinske akcije Povlačenje uređaja i Brisanje uređaja mogu se koristiti za uklanjanje podataka tvrtke kojima upravlja Intune ili za vraćanje na tvorničke postavke i vraćanje uređaja na zadane postavke.

1. Prijavite se u Microsoft 365 upravljanje uređajima pa idite na **Uređaji**  >  **Svi uređaji**.
2. Odaberite uređaj koji želite izbrisati.
3. Odaberite vrstu daljinskog brisanja koju želite učiniti. Povlačenjem se brišu samo podaci tvrtke ili ustanove, a potpuno brisanje uređaja vraća na tvorničke postavke.
4. Odaberite **Da** da biste potvrdili. Dok brisanje ne završi, status akcije Uređaj prikazuje se kao Povlačenje *na čekanju.*
    Kada akcija završi, mobilni uređaj više se neće vidjeti na popisu upravljanih uređaja.

> [!NOTE]
> Podaci tvrtke ne mogu se ukloniti s uređaja pridruženih servisu Azure AD. 

Potpune pojedinosti o efektu akcija Povlačenje i brisanje, uključujući ono što se zadržava i što se briše, potražite u sljedećoj dokumentaciji:

- [Uklonite uređaje brisanjem, povlačenjem ili ručnim poništavanjem uređaja.](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)
- [Brisanje samo korporativnih podataka iz aplikacija kojima upravlja Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Brisanje svih podataka s uređaja sa sustavom macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).