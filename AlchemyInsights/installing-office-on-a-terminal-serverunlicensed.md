---
title: Instalacija sustava Office na Terminal Server – nelicencirani
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663109"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalacija sustava Office na Terminal Server

Za implementaciju Microsoft 365 aplikacija za Enterprise na sustavu Windows Server pomoću servisa udaljene radne površine (RDS-a), prijašnjeg naziva terminalskih servisa:
  
- Morate imati pretplatu na Microsoft 365 koja obuhvaća aplikacije Microsoft 365 za Enterprise, kao što je Office 365 Enterprise E3 ili Enterprise E5. Tarife Microsoft 365 za tvrtke i Microsoft 365 Apps za Business Premium ne obuhvaćaju aplikacije Microsoft 365 za Enterprise.

- Morate omogućiti [zajedničko korištenje računala](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ako želite instalirati aplikacije Microsoft 365 za Enterprise na RDS-u iz centra za administratore sustava Microsoft 365, ***koji koristi zadane postavke instalacije***, slijedite sljedeće korake.

> [!TIP]
> Možete i preuzeti i pokrenuti pomoćnik za [Microsoftove podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) da biste instalirali Microsoft 365 Apps za Enterprise u načinu rada za zajedničko korištenje računala.
  
1. Provjerite koju pretplatu na Microsoft 365 imate. [Naučite kako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ako je potrebno, prijeđite na drugu pretplatu na Microsoft 365. [Naučite kako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ako je Office već instaliran na RDS poslužitelju pomoću bilo koje druge pretplate na Microsoft 365, deinstalirajte ga. Na primjer, ako odete na upravljačku ploču, \> deinstalirajte program. Deinstalirajte pomoću [Microsoftova pomoćnika za podršku i oporavak Ako nailazite](https://aka.ms/SARA-OfficeUninstall-Alchemy) na probleme.

4. Na RDS poslužitelju prijavite se u centar za administratore sustava Microsoft 365 s administratorskim računom i [Instalirajte aplikacije microsoft 365 za Enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Nakon instalacije sustava Office ***ne otvarajte ni ne prijavljujte se u*** bilo koju aplikaciju sustava Office.

6. Na RDS poslužitelju omogućite aktivaciju pomoću zajedničkog računala uređivanjem registra slijedeći ove korake:

1. Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona, a zatim odaberite Pokreni. U okvir Otvori upišite **regedit**, a zatim odaberite u redu.

2. Kada se od vas zatraži da omogućite uređivaču registra da biste unijeli promjene na uređaju, odaberite da.

3. U uređivaču registra dodajte vrijednost niza programa **Sharedcomputerlicenciranje** s postavkom 1 u odjeljku HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na RDS poslužitelju prijavite se ***kao krajnji korisnik*** i [Provjerite je li aktivacija zajedničkog računala omogućena za aplikacije Microsoft 365 za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Dodatne informacije o preduvjetima, uputama za postavljanje i smjernicama o prilagođenim instalacijama pomoću alata za implementaciju sustava Office potražite u članku [Implementacija aplikacija Microsoft 365 za Enterprise pomoću servisa udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Da biste riješili pogreške povezanih s aktivacijom zajedničkog računala, pročitajte članak [Otklanjanje poteškoća s aktivacijom zajedničkog računala za aplikacije Microsoft 365 za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  