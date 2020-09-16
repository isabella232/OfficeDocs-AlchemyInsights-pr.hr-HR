---
title: Problemi pomoću konzole Intune admin
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
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728279"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemi pomoću konzole Intune admin

**"Pristup je odbijen" prilikom navigacije putem portala Intune admin.**

- Ako ste član prilagođene uloge u ugodi, provjerite je li vaš račun dodijeljen licencama za Intune ili Enterprise Mobility suite (EMS).
- Ako upraviteljem konfiguracije koristite za upravljanje uređajima, provjerite niste li dio zbirke dodatka user za Configuration Manager MDM.
- Provjerite jesu li vam dodijeljene dozvole za upravljanje administracijom na temelju uloga (RBAC) u oštrici Intune uloge.
- Provjera korištene grupe nije popis za raspodjelu. Intune na portalu Azure podržava samo korisničke račune koji spadaju u sigurnosne grupe servisa Azure Active Directory. Pregledajte grupe na portalu Azure > **Intune**  >  **Groups**ili na portalu Azure > **Azure Active Directory**.

**Korisnik ima previše dozvola za dodijeljenu ulogu Utune.**

Savjetujte korisniku da se otvori u odjeljku **Intune**  >  **Intune**za  >  **moje dozvole**  >  za**Izvoz** da biste pregledali dodijeljene dozvole.

**U ulogu sam dodao grupu opsega, no korisnici u toj ulozi i dalje vide druge korisnike ili uređaje.**

Grupe dosega ne filtriraju korisnike ni uređaje. Grupe dosega:

- Ograničite osobe kojima korisnici mogu dodijeliti pravila ili aplikacije.
- Dopusti samo određenim korisnicima pokretanje udaljenih zadataka na uređajima.

Dodatne informacije o grupama dosega potražite u članku  [kontrola pristupa utemeljenoj na ulogama (RBAC) pomoću aplikacije Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Dodao sam korisnika u željenu ulogu, ali i dalje imaju potpun pristup konzoli za administraciju Intune.**

Idite na Umetanje > **korisnika** na portalu Azure i provjerite nije li korisnik dodijeljen bilo kojoj od sljedećih uloga na portalu Azure:

- Globalni administrator
- Unos administratora usluge
- Administrator sustava SharePoint

Dodatne informacije potražite u članku [kontrola pristupa utemeljenu na ulogama (RBAC) pomoću aplikacije Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemi s pristupom**

Dodatne informacije potražite u članku [ne možete se prijaviti u Office 365, Azure ili Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).