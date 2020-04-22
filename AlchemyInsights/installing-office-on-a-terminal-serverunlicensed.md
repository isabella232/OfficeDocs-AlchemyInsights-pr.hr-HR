---
title: Instalacija sustava na terminalski poslužitelj – bez licence
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
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763209"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalacija sustava Office na terminalski poslužitelj

Za implementaciju aplikacija microsoft 365 za tvrtke na Windows Server pomoću servisa Udaljene radne površine (RDS), ranije nazvane Terminal Services:
  
- Morate imati pretplatu na Microsoft 365 koja obuhvaća Aplikacije sustava Microsoft 365 za tvrtke, kao što su Office 365 Enterprise E3 ili Enterprise E5. Tarife Microsoft 365 Apps for business i Microsoft 365 Apps for business Premium ne obuhvaćaju Aplikacije za Microsoft 365 za tvrtke.

- Morate omogućiti [aktivaciju dijeljenog računala](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Ako želite instalirati Microsoft 365 aplikacije za tvrtke na RDS iz centra za administratore sustava Microsoft 365, ***koji koristi zadane postavke instalacije,*** slijedite ove korake.

> [!TIP]
> Microsoftov [pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) možete preuzeti i pokrenuti da biste instalirali Microsoft 365 Aplikacije za tvrtke u načinu aktivacije dijeljenog računala.
  
1. Provjerite koju pretplatu na Microsoft 365 imate. [Saznajte kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Ako je potrebno, prijeđite na drugu pretplatu na Microsoft 365. [Saznajte kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Ako je Office već instaliran na RDS poslužitelju pomoću bilo koje druge pretplate na Microsoft 365, deinstalirajte ga. Na primjer, tako da \> odete na Upravljačku ploču Deinstalirajte program. Ako imate problema, deinstalirajte pomoću [Microsoftova pomoćnika za podršku i oporavak.](https://aka.ms/SARA-OfficeUninstall-Alchemy)

4. Na RDS poslužitelju prijavite se u centar za administratore sustava Microsoft 365 pomoću administratorskog računa i [instalirajte Microsoft 365 Apps za tvrtke](https://portal.office.com/OLS/MySoftware.aspx).

5. Nakon instalacije sustava Office ***nemojte otvarati aplikacije*** sustava Office niti se prijaviti u ih.

6. Na RDS poslužitelju omogućite aktivaciju zajedničkog računala uređivanjem registra slijedeći ove korake:

1. Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite Pokreni. U okvir Otvori upišite **regedit**, a zatim odaberite U redu.

2. Odaberite Da kada se od vas zatraži da dopustite uređivaču registra da unese promjene na uređaj.

3. In Registry Editor, dodati vrpca vrijednost od **SharedComputerLicensing** sa postavljanje od 1 pod HKEY_LOCAL_MACHINESOFTWAREMicrosoftOfficeClickToRunConfiguration\\\\.

7. Na RDS poslužitelju ***prijavite se kao krajnji korisnik*** i provjerite je li [aktivacija zajedničkog računala omogućena za Microsoft 365 Aplikacije za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Dodatne informacije o preduvjetima, uputama za postavljanje i smjernicama o prilagođenim instalacijama pomoću alata za implementaciju sustava Office [potražite u članku Implementacija aplikacija microsoft 365 za tvrtke pomoću servisa Udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Da biste ispravili pogreške vezane uz aktivaciju zajedničkog računala, [pročitajte članak Otklanjanje poteškoća s aktivacijom zajedničkog računala za Aplikacije sustava Microsoft 365 za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  