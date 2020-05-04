---
title: Implementacija aplikacija microsoft 365 za tvrtke za zajedničko korištenje na RDS-u, terminalskom poslužitelju ili VDI-u
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 51512b29f8d37ce6c39ece5bb704cb01e88e463d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010246"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementacija aplikacija microsoft 365 za tvrtke za zajedničko korištenje na RDS-u, terminalskom poslužitelju ili VDI-u

Da biste implementirali Microsoft 365 aplikacije za tvrtke pomoću servisa Udaljene radne površine (RDS), koji su prethodno nazivali Servisterminal:
- Morate imati tarifu za Microsoft 365 For Business ili tarifu za Office 365 koja obuhvaća aplikacije Microsoft 365 za tvrtke, kao što su Office 365 Enterprise E3 ili Enterprise E5.
   > [!NOTE] 
   > Tarife Microsoft 365 Apps for business i Microsoft 365 Business Premium Standard ne obuhvaćaju Aplikacije sustava Microsoft 365 za tvrtke.
- Morate omogućiti [aktivaciju dijeljenog računala](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Microsoftov [pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) možete preuzeti i pokrenuti da biste instalirali Microsoft 365 Aplikacije za tvrtke u načinu aktivacije dijeljenog računala.

Dodatne informacije o preduvjetima, uputama za postavljanje i smjernicama o prilagođenim instalacijama pomoću alata za implementaciju sustava Office [potražite u članku Implementacija aplikacija microsoft 365 za tvrtke pomoću servisa udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Da biste ispravili pogreške povezane s aktivacijom zajedničkog računala:
- Pročitajte [članak Otklanjanje poteškoća s aktivacijom zajedničkog računala za Microsoft 365 aplikacije za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Pročitajte članak [Resetiranje aplikacija sustava Microsoft 365 za stanje aktivacije za velike tvrtke](https://go.microsoft.com/fwlink/?linkid=2109218).

Ako želite instalirati Microsoft 365 aplikacije za tvrtke na RDS iz centra za administratore sustava Microsoft 365, ***koji koristi zadane postavke instalacije,*** slijedite ove korake:

1.    Provjerite koju pretplatu imate. [Saznajte kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Ako je potrebno, prijeđite na drugu pretplatu. [Saznajte kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Ako je Office već instaliran na RDS poslužitelju pomoću bilo koje druge Microsoftove pretplate, deinstalirajte ga. Na primjer, tako da odete na **Upravljačku ploču** > **Deinstalirajte program**. Ako imate problema, deinstalirajte pomoću [Microsoftova pomoćnika za podršku i oporavak.](https://aka.ms/SARA-OfficeUninstall-Alchemy)
4.    Na RDS poslužitelju prijavite se u centar za administratore sustava Microsoft 365 pomoću administratorskog računa i [instalirajte Microsoft 365 Apps za tvrtke](https://portal.office.com/OLS/MySoftware.aspx).
5.    Nakon instalacije sustava Office ***nemojte otvarati aplikacije*** sustava Office niti se prijaviti u ih.
6.    Na RDS poslužitelju omogućite aktivaciju zajedničkog računala uređivanjem registra slijedeći ove korake:
   1. Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite **Pokreni**. U okvir Otvori upišite **regedit**, a zatim odaberite **U redu**.
   2. Odaberite **Da** kada se od vas zatraži da dopustite uređivaču registra da unese promjene na uređaj.
   3. In Registry Editor, dodati vrpca vrijednost od **SharedComputerLicensing** sa postavljanje od 1 pod HKEY_LOCAL_MACHINESOFTWAREMicrosoftOfficeClickToRunConfiguration\\\\.
   4. Na RDS poslužitelju ***prijavite se kao krajnji korisnik*** i provjerite je li [aktivacija zajedničkog računala omogućena za Microsoft 365 Aplikacije za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

