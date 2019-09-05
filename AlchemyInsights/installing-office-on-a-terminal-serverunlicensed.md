---
title: Instaliranje sustava office na Terminal Serveru - nelicenciran
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735381"
---
# <a name="installing-office-on-a-terminal-server"></a>Instaliranje sustava Office na terminalski poslužitelj

Za uvođenje Office 365 ProPlus na poslužitelju Windows pomoću udaljene radne površine Services (ZAPISI), prije naziva servisa Terminal Services:
  
- Morate imati Office 365 plan koji uključuje Office 365 ProPlus, kao što je Office 365 Enterprise E3 ili Enterprise E5. Planovi poslovnih Office 365 i Office 365 poslovne Premium uključuju Office 365 ProPlus.

- Morate omogućiti [zajedničko računalo aktivacije](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Ako želite instalirati Office 365 ProPlus ZAPISI iz centra admin Microsoft 365 ***koji koristi zadane postavke instalacije***, slijedite ove korake:
  
1. Provjerite što Office 365 plan imate. [Saznajte kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Ako je potrebno, prijeđite na drugu Office 365 plan. [Saznajte kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Office već instaliran na poslužitelju ZAPISI pomoću Office 365 planove, deinstalirajte ga. Na primjer, odlaskom na upravljačkoj ploči \> deinstalirati program. Deinstaliraj pomoću [Microsoft podršku i oporavak pomoćnika](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako se izvodi u problemi.

4. Na poslužitelju ZAPISI prijaviti u Centar za administraciju Microsoft 365 s administratorskog računa i [instalirajte Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Nakon instalacije Officea ***ne otvorite ili prijaviti*** za sve Officeove aplikacije.

6. Na poslužitelju ZAPISI omogućili aktivaciju dijeljenom računalu uređivanjem registra slijedeći ove korake:

1. Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite Pokreni. U okvir Otvori upišite **regedit**, a zatim odaberite u redu.

2. Odaberite da upit o dozvoli uređivač registra da biste napravili promjene na uređaj.

3. U uređivač registra, dodajte vrijednost niza **SharedComputerLicensing** s postavkom 1 pod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na poslužitelju ZAPISI, ***prijavite se kao krajnji korisnik*** i [Provjerite je li aktivacija dijeljenom računalu omogućen za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Za dodatne pojedinosti o preduvjeti, upute za postavljanje i prilagođene instalacije pomoću alata za uvođenje Office upute pogledajte [Uvođenje Office 365 ProPlus pomoću udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Da biste riješili pogreške vezane uz aktivaciju dijeljenom računalu, pogledajte [otklanjanje problema s dijeljenom računalu aktivacije za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  