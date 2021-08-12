---
title: Problemi s korištenjem administratorske konzole Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 9310e8685a922207be8d5672d7929e19313cbb57e0fa6d25de149106692e811f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944123"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemi s korištenjem administratorske konzole Intune

**"Access denied" (Pristup je odbijen) prilikom navigacije portalom za administratore aplikacije Intune.**

- Ako ste član prilagođene uloge aplikacije Intune, provjerite je li na vašem računu dodijeljena licenca Intune ili Enterprise Mobility Suite (EMS).
- Ako za upravljanje uređajima koristite Upravitelj konfiguracije, provjerite niste li dio korisničke zbirke intune za MDM upravitelja konfiguracije.
- Provjerite jesu li vam dodijeljene odgovarajuće dozvole za administraciju utemeljenu na ulogama (RBAC) na oštrici uloga Intune.
- Provjerite nije li korištena grupa popis za raspodjelu. Intune na portalu Azure podržava samo korisničke račune koji pripadaju Azure Active Directory sigurnosnim grupama. Pregledajte grupe na portalu Azure > **Intune**  >  **Groups** ili na portalu Azure > **Azure Active Directory**.

**Korisnik ima previše dozvola za dodijeljenu ulogu intune**

Savjetujte korisnika da ode na **Intune**  >  **Intune uloge**  >  **Moje dozvole**  >  **Izvoz** da biste pregledali odobrene dozvole.

**U ulogu sam dodao grupu opsega, ali korisnici u toj ulozi i dalje vide druge korisnike ili uređaje.**

Grupe opsega ne filtriraju korisnike ni uređaje. Grupe opsega:

- Ograničite korisnike kojima korisnici mogu dodijeliti pravilnike ili aplikacije.
- Dopustite samo određenim korisnicima pokretanje udaljenih zadataka na uređajima.

Dodatne informacije o grupama opsega potražite u članku Kontrola pristupa [utemeljena na ulogama (RBAC) s Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Dodao sam korisnika u ulogu aplikacije Intune, ali i dalje ima puni pristup administratorskim konzolama intune.**

Otvorite Intune > **na** portalu Azure i provjerite nije li korisniku dodijeljena sljedeća uloga na portalu Azure:

- Globalni administrator
- Administrator servisa Intune
- SharePoint administrator

Dodatne informacije potražite u članku [Kontrola pristupa utemeljena na ulogama (RBAC) s Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemi s pristupom**

Dodatne informacije potražite u članku Ne možete se prijaviti na [Office 365, Azure ili Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).