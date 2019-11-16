---
title: Instaliranje ureda na terminalskom poslužitelju-Nelicencirano
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37205401"
---
# <a name="installing-office-on-a-terminal-server"></a>Instaliranje Officea na terminalskom poslužitelju

Za uvođenje sustava Office 365 ProPlus na Windows Server pomoću usluga udaljene radne površine (RDS), ranije imena Terminal Services:
  
- Morate imati Office 365 plan koji uključuje Office 365 ProPlus, kao što su Office 365 Enterprise E3 ili Enterprise E5. Planovi Office 365 Business i Office 365 Business Premium ne uključuju Office 365 ProPlus.

- Morate omogućiti [aktivaciju zajedničkog računala](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Ako želite instalirati Office 365 ProPlus na RDS iz centra Microsoft 365 admin, ***koji koristi zadane instalacije postavke***, koristite sljedeće korake.

> [!TIP]
> Također možete preuzeti i pokrenuti [Microsoftov pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) da biste instalirali Office 365 proplus u načinu rada za aktivaciju zajedničkog računala.
  
1. Provjerite koji Office 365 plan imate. [Naučite kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Ako je potrebno, prebacite se na drugi Office 365 plan. [Naučite kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Ako je Office već instaliran na poslužitelju RDS pomoću bilo kojeg drugog Office 365 planova, deinstalirati ga. Na primjer, ako idete na Upravljačka ploča \> deinstalirati program. Deinstalirajte pomoću [Microsoftove podrške i oporavka od pomoćnika](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako ste u problemima.

4. Na RDS poslužitelju, prijavite se na Microsoft 365 Admin Center s administratorskim računom i [instalirajte Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Nakon instalacije sustava Office ***Nemojte otvarati ili se prijaviti u*** bilo koje aplikacije sustava Office.

6. Na RDS poslužitelju omogućite zajedničko računalo aktivaciju uređivanjem registra slijedeći ove korake:

1. Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite Pokreni. U okvir Otvori upišite **regedit**, a zatim odaberite u redu.

2. Odaberite da kada se od vas zatraži da omogućite uređivač registra da napravi promjene na uređaju.

3. U uređivaču registra dodajte vrijednost niza **Sharedcomputer,** uz postavku 1 u odjeljku HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na RDS poslužitelju prijavite se ***kao krajnji korisnik*** i [Provjerite je li aktivacija zajedničkog računala omogućena za Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Za više detalja o preduvjeta, upute za postavljanje i smjernice o prilagođenim instalacijama pomoću alata za implementaciju sustava Office potražite u [instalaciji sustava office 365 ProPlus pomoću usluga udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Da biste riješili pogreške povezane s aktivacijom zajedničkog računala, pogledajte [Rješavanje problema s aktivacijom zajedničkog računala za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  