---
title: Implementacija Office 365 ProPlus za zajedničko korištenje na RDS, Terminal Server, ili VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959452"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementacija Office 365 ProPlus za zajedničko korištenje na RDS, Terminal Server, ili VDI

Da biste implementirati Office 365 ProPlus pomoću usluga udaljene radne površine (RDS), ranije imena Terminal Services:
- Morate imati Microsoft 365 za Business plan ili Office 365 plan koji uključuje Office 365 ProPlus, kao što su Office 365 Enterprise E3 ili Enterprise E5.
   > [!NOTE] 
   > Planovi Office 365 Business i Office 365 Business Premium ne uključuju Office 365 ProPlus.
- Morate omogućiti [aktivaciju zajedničkog računala](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Također možete preuzeti i pokrenuti [Microsoftov pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) da biste instalirali Office 365 proplus u načinu rada za aktivaciju zajedničkog računala.

Dodatne informacije o preduvjete, uputama za postavljanje i smjernicama o prilagođenim instalacijama pomoću alata za implementaciju sustava Office potražite u uputi [office 365 ProPlus pomoću usluga udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Da biste riješili pogreške povezane s aktivacijom zajedničkog računala:
- Pogledajte [Rješavanje problema s aktivacijom zajedničkog računala za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Pogledajte [reset Office 365 ProPlus stanje aktivacije](https://go.microsoft.com/fwlink/?linkid=2109218).

Ako želite instalirati Office 365 ProPlus na RDS iz centra Microsoft 365 admin, ***koji koristi zadane instalacije postavke***, koristite sljedeće korake:

1.  Provjerite koji Office 365 plan imate. [Nauči kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Ako je potrebno, prebacite se na drugi Office 365 plan. [Nauči kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Ako je Office već instaliran na poslužitelju RDS pomoću bilo kojeg drugog Office 365 planova, deinstalirati ga. Na primjer, idete na **upravljačku ploču** > **deinstalirati program**. Deinstalirajte pomoću [Microsoftove podrške i oporavka od pomoćnika](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako ste u problemima.
4.  Na RDS poslužitelju, prijavite se na Microsoft 365 Admin Center s administratorskim računom i [instalirajte Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Nakon instalacije sustava Office ***Nemojte otvarati ili se prijaviti u*** bilo koje aplikacije sustava Office.
6.  Na RDS poslužitelju omogućite zajedničko računalo aktivaciju uređivanjem registra slijedeći ove korake:
   1. Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite **Pokreni**. U okvir Otvori upišite **regedit**, a zatim odaberite **u redu**.
   2. Odaberite **da** kada se od vas zatraži da omogućite uređivač registra da napravi promjene na uređaju.
   3. U uređivaču registra dodajte vrijednost niza **Sharedcomputer,** uz postavku 1 u odjeljku HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na RDS poslužitelju prijavite se ***kao krajnji korisnik*** i [Provjerite je li aktivacija zajedničkog računala omogućena za Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

