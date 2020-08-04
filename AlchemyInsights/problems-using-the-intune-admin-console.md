---
title: Problemi s korištenjem konzole administratora Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554881"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemi s korištenjem konzole administratora Intune

**"Pristup je odbijen" prilikom navigacije intune admin portalom.**

- Ako ste član prilagođene uloge Intune, provjerite je li vaš račun dodijeljena licenca Intune ili Enterprise Mobility Suite (EMS).
- Ako koristite Upravitelj konfiguracije za upravljanje uređajima, provjerite niste li dio zbirke korisnika Intune za Upravitelj konfiguracije MDM.
- Provjerite jesu li vam dodijeljene odgovarajuće dozvole kontrole administracije temeljene na ulogama (RBAC) u oštrici uloga Intune.
- Provjerite da korištena grupa nije popis raspodjele. Intune na portalu Azure podržava samo korisničke račune koji pripadaju sigurnosnim grupama servisa Azure Active Directory. Pregledajte grupe na portalu Azure > **Intune**  >  **Groups**ili na portalu Azure > **Azure Active Directory**.

**Korisnik ima previše dozvola za dodijeljenu ulogu Intune**

Savjetovati korisnika da ide **na Intune**  >  **Intune uloge**  >  **Moje dozvole**  >  **Izvoz** pregledati odobrene dozvole.

**Dodala sam grupu dosega ulozi, ali korisnici u toj ulozi i dalje vide druge korisnike ili uređaje.**

Grupe dosega ne filtriraju korisnike ili uređaje. Grupe dosega:

- Ograničite kome korisnici mogu dodijeliti pravila ili aplikacije.
- Dopustite samo određenim korisnicima pokretanje daljinskih zadataka na uređajima.

Dodatne informacije o grupama dosega [potražite u odjeljku Kontrola pristupa utemeljena na ulogama (RBAC) s programom Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**JA dodani korisnik to Intune uloga ali oni pa ipak imati pun pristup to Intune admin utješiti.**

Idite na Intune > **korisnici na** portalu Azure i provjerite nije li korisnik dodijeljen nijednoj od sljedećih uloga na portalu Azure:

- Globalni administrator
- Intune administrator usluga
- Administrator sustava SharePoint

Dodatne informacije [potražite u odjeljku Kontrola pristupa temeljena na ulogama (RBAC) s programom Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemi s pristupom**

Dodatne informacije [potražite u odjeljku Ne možete se prijaviti u Office 365, Azure ili Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).