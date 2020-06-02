---
title: Instaliranje ureda na terminalskom poslužitelju - Nelicencirana
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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508620"
---
# <a name="installing-office-on-a-terminal-server"></a>Instaliranje sustava Office na terminalski poslužitelj

Za implementaciju aplikacija sustava Microsoft 365 za tvrtke na Windows Serveru pomoću servisa udaljene radne površine (RDS), koji su prethodno imenovani servisima Terminal Services:
  
- Morate imati pretplatu na Microsoft 365 koja obuhvaća Aplikacije microsoft 365 za tvrtke, kao što su Office 365 Enterprise E3 ili Enterprise E5. Tarife za Microsoft 365 aplikacije za tvrtke i Microsoft 365 Aplikacije za tvrtke Premium ne obuhvaćaju Microsoft 365 Aplikacije za tvrtke.

- Morate omogućiti [aktivaciju dijeljenog računala](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ako želite instalirati Microsoft 365 Apps za poduzeće na RDS iz centra za administratore sustava Microsoft 365, ***koji koristi zadane postavke instalacije, slijedite***ove korake.

> [!TIP]
> [Microsoftov pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) možete preuzeti i pokrenuti da biste instalirali Microsoft 365 Apps za tvrtke u načinu aktivacije dijeljenog računala.
  
1. Provjerite imate li pretplatu na Microsoft 365. [Saznajte kako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ako je potrebno, prijeđite na drugu pretplatu na Microsoft 365. [Saznajte kako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ako je Office već instaliran na RDS poslužitelju pomoću bilo koje druge pretplate na Microsoft 365, deinstalirajte je. Na primjer, tako da odete na \> Deinstalaciju programa na upravljačkoj ploči. Deinstalirajte pomoću [Microsoftova pomoćnika za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako naišate na probleme.

4. Na RDS poslužitelju prijavite se u centar za administratore sustava Microsoft 365 pomoću administratorskog računa i [instalirajte Microsoft 365 Apps za tvrtke](https://portal.office.com/OLS/MySoftware.aspx).

5. Nakon instalacije sustava Office ***nemojte otvarati niti se prijavjeti u*** bilo koje aplikacije sustava Office.

6. Na RDS poslužitelju omogućite aktivaciju zajedničkog računala uređivanjem registra slijedeći ove korake:

1. Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite Pokreni. U okvir Otvori upišite **regedit**, a zatim odaberite U redu.

2. Odaberite Da kada se to od vas zatraži da dopustite uređivaču registra da unesete promjene na uređaju.

3. U uređivaču registra dodajte vrijednost niza **SharedComputerLicensing** s postavkom 1 pod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na RDS poslužitelju ***prijavite se kao krajnji korisnik*** i provjerite je li [aktivacija dijeljenog računala omogućena za Microsoft 365 Apps za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Dodatne informacije o preduvjetima, uputama za postavljanje i smjernicama o prilagođenim instalacijama pomoću alata za implementaciju sustava Office potražite [u članku Implementacija aplikacija microsoft 365 za tvrtke pomoću servisa udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Da biste ispravili pogreške povezane s aktivacijom dijeljenog računala, [pročitajte članak Otklanjanje poteškoća s aktivacijom dijeljenog računala za Aplikacije Microsoft 365 za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  