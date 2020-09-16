---
title: Implementacija aplikacija Microsoft 365 za Enterprise za zajedničko korištenje na RDS-u, terminalskom poslužitelju ili VDI-u
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745527"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementacija aplikacija Microsoft 365 za Enterprise za zajedničko korištenje na RDS-u, terminalskom poslužitelju ili VDI-u

Da biste implementirali Microsoftove 365 aplikacije za Enterprise pomoću servisa udaljene radne površine (RDS-a), prethodno imenovani Terminal Services:
- Morate imati plan Microsoft 365 za tvrtke ili plan sustava Office 365 koji obuhvaća aplikacije Microsoft 365 za Enterprise, kao što je Office 365 Enterprise E3 ili Enterprise E5.
   > [!NOTE] 
   > U programima Microsoft 365 Apps za tvrtke i Microsoft 365 Business Premium standardne tarife ne obuhvaćaju aplikacije Microsoft 365 za Enterprise.
- Morate omogućiti [zajedničko korištenje računala](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Možete i preuzeti i pokrenuti pomoćnik za [Microsoftove podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) da biste instalirali Microsoft 365 Apps za Enterprise u načinu rada za zajedničko korištenje računala.

Dodatne informacije o preduvjetima, uputama za postavljanje i smjernicama o prilagođenim instalacijama pomoću alata za implementaciju sustava Office potražite u članku [Implementacija aplikacija Microsoft 365 za Enterprise pomoću servisa udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Da biste riješili pogreške vezane uz aktivaciju zajedničkog računala, učinite sljedeće:
- Pročitajte članak [Otklanjanje poteškoća s aktivacijom zajedničkog računala za aplikacije Microsoft 365 za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Pročitajte članak [Resetiranje aplikacija sustava Microsoft 365 za stanje aktivacije za velike tvrtke](https://go.microsoft.com/fwlink/?linkid=2109218).

Ako želite instalirati aplikacije Microsoft 365 za Enterprise na RDS-u iz centra za administratore sustava Microsoft 365, ***koje koristi zadane postavke instalacije***, slijedite sljedeće korake:

1.    Provjerite koju pretplatu imate. [Naučite kako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Ako je potrebno, prijeđite na drugu pretplatu. [Naučite kako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Ako je Office već instaliran na RDS poslužitelju pomoću ostalih Microsoftovih pretplata, deinstalirajte ga. Na primjer, ako odete na **upravljačku ploču**,  >  **deinstalirajte program**. Deinstalirajte pomoću [Microsoftova pomoćnika za podršku i oporavak Ako nailazite](https://aka.ms/SARA-OfficeUninstall-Alchemy) na probleme.
4.    Na RDS poslužitelju prijavite se u centar za administratore sustava Microsoft 365 s administratorskim računom i [Instalirajte aplikacije microsoft 365 za Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    Nakon instalacije sustava Office ***ne otvarajte ni ne prijavljujte se u*** bilo koju aplikaciju sustava Office.
6.    Na RDS poslužitelju omogućite aktivaciju pomoću zajedničkog računala uređivanjem registra slijedeći ove korake:
   1. Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona, a zatim odaberite **Pokreni**. U okvir Otvori upišite **regedit**, a zatim odaberite **u redu**.
   2. Kada se od vas zatraži da omogućite uređivaču registra da biste unijeli promjene na uređaju, odaberite **da** .
   3. U uređivaču registra dodajte vrijednost niza programa **Sharedcomputerlicenciranje** s postavkom 1 u odjeljku HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na RDS poslužitelju prijavite se ***kao krajnji korisnik*** i [Provjerite je li aktivacija zajedničkog računala omogućena za aplikacije Microsoft 365 za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

