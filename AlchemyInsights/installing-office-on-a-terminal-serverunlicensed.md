---
title: Instalacija sustava Office na terminalski poslužitelj – nelicencirani
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
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055150"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalacija Office na terminalski poslužitelj

Za implementaciju Microsoft 365 Apps za velike tvrtke na Windows poslužitelja putem servisa Remote Desktop Services (RDS), nekadašnjeg imena Servisi terminala:
  
- Morate imati pretplatu Microsoft 365 koja obuhvaća Microsoft 365 Apps za velike tvrtke, kao što su Office 365 Enterprise E3 ili Enterprise E5. Planovi Microsoft 365 Apps za male tvrtke i Microsoft 365 Apps za male tvrtke premium ne obuhvaćaju Microsoft 365 Apps za velike tvrtke.

- Morate omogućiti aktivaciju [zajedničkog računala](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ako želite instalirati Microsoft 365 Apps za velike tvrtke RDS iz Centar za administratore okruženja Microsoft 365, koji koristi zadane ***postavke instalacije,*** slijedite korake u nastavku.

> [!TIP]
> Možete i preuzeti i pokrenuti Microsoft pomoćnik za podršku i oporavak [da biste Microsoft 365 Apps za velike tvrtke](https://aka.ms/SaRA_OfficeSCA_M365Portal) u načinu aktivacije zajedničkog računala.
  
1. Provjerite koju Microsoft 365 pretplatu imate. [Saznajte kako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ako je potrebno, prijeđite na drugu Microsoft 365 pretplatu. [Saznajte kako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ako Office već instaliran na RDS poslužitelju pomoću bilo koje druge Microsoft 365 pretplate, deinstalirajte ga. Na primjer, e-pošte na upravljačkoj \> ploči Deinstalirajte program. [Deinstalacija pomoću pomoćnik za podršku i oporavak ako](https://aka.ms/SARA-OfficeUninstall-Alchemy) naiđete na probleme.

4. Na RDS poslužitelju prijavite se na Centar za administratore okruženja Microsoft 365 pomoću administratorskog računa i [instalirajte Microsoft 365 Apps za velike tvrtke](https://portal.office.com/OLS/MySoftware.aspx).

5. Kada Office instalirate, ***nemojte se otvarati ni prijaviti u*** bilo koju Office aplikacije.

6. Na RDS poslužitelju omogućite aktivaciju zajedničkog računala uređivanjem registra na sljedeći način:

1. Desnom tipkom miša kliknite Windows u donjem lijevom kutu zaslona pa odaberite Pokreni. U okvir Otvori upišite **regedit**, a zatim odaberite U redu.

2. Odaberite Da kada se od vas zatraži da omogućite uređivaču registra da unosi promjene na uređaj.

3. U uređivač registra dodajte vrijednost niza za **SharedComputerLicensing** s postavkom 1 u odjeljku HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na RDS poslužitelju prijavite se kao krajnji ***korisnik i*** provjerite je li omogućena [aktivacija](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)zajedničkog računala za Microsoft 365 Apps za velike tvrtke .

Dodatne informacije o preduvjetima, uputama za postavljanje i smjernicama o prilagođenim instalacijama pomoću alata za implementaciju sustava Office potražite u [članku Implementacija Microsoft 365 Apps za velike tvrtke pomoću](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)servisa udaljene radne površine .
  
Da biste ispravili pogreške povezane s aktivacijom zajedničkog računala, pročitajte otklanjanje [poteškoća s aktivacijom zajedničkog računala Microsoft 365 Apps za velike tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  