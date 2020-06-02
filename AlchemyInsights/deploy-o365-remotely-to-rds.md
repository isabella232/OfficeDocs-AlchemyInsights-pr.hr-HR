---
title: Implementacija aplikacija sustava Microsoft 365 za tvrtke za zajedničko korištenje na RDS-u, terminalskom poslužitelju ili VDI-u
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
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507578"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementacija aplikacija sustava Microsoft 365 za tvrtke za zajedničko korištenje na RDS-u, terminalskom poslužitelju ili VDI-u

Da biste implementirali Microsoft 365 aplikacije za tvrtke pomoću servisa udaljene radne površine (RDS), a prethodno nazvane Servisi terminala:
- Morate imati tarifu Microsoft 365 For Business ili tarifu za Office 365 koja obuhvaća Aplikacije microsoft 365 za tvrtke, kao što su Office 365 Enterprise E3 ili Enterprise E5.
   > [!NOTE] 
   > Planovi Microsoft 365 Apps for business i Microsoft 365 Business Premium Standard ne obuhvaćaju Microsoft 365 Aplikacije za tvrtke.
- Morate omogućiti [aktivaciju dijeljenog računala](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> [Microsoftov pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) možete preuzeti i pokrenuti da biste instalirali Microsoft 365 Apps za tvrtke u načinu aktivacije dijeljenog računala.

Dodatne informacije o preduvjetima, uputama za postavljanje i smjernicama o prilagođenim instalacijama pomoću alata za implementaciju sustava Office potražite [u članku Implementacija aplikacija microsoft 365 za tvrtke pomoću servisa udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Da biste ispravili pogreške vezane uz aktivaciju dijeljenog računala:
- Pogledajte [Otklanjanje poteškoća s aktivacijom dijeljenog računala za Microsoft 365 Apps za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Pročitajte članak [Resetiranje aplikacija sustava Microsoft 365 za stanje aktivacije za velike tvrtke](https://go.microsoft.com/fwlink/?linkid=2109218).

Ako želite instalirati Microsoft 365 Apps za poduzeće na RDS iz centra za administratore sustava Microsoft 365, ***koji koristi zadane postavke instalacije,*** slijedite ove korake:

1.    Provjerite koju pretplatu imate. [Saznajte kako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Ako je potrebno, prijeđite na drugu pretplatu. [Saznajte kako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Ako je Office već instaliran na RDS poslužitelju pomoću bilo koje druge Microsoftove pretplate, deinstalirajte ga. Na primjer, tako da odete na **Upravljačka ploča**  >  **Deinstalirajte program**. Deinstalirajte pomoću [Microsoftova pomoćnika za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako naišate na probleme.
4.    Na RDS poslužitelju prijavite se u centar za administratore sustava Microsoft 365 pomoću administratorskog računa i [instalirajte Microsoft 365 Apps za tvrtke](https://portal.office.com/OLS/MySoftware.aspx).
5.    Nakon instalacije sustava Office ***nemojte otvarati niti se prijavjeti u*** bilo koje aplikacije sustava Office.
6.    Na RDS poslužitelju omogućite aktivaciju zajedničkog računala uređivanjem registra slijedeći ove korake:
   1. Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite **Pokreni**. U okvir Otvori upišite **regedit**, a zatim odaberite **U redu**.
   2. Odaberite **Da** kada se to od vas zatraži da dopustite uređivaču registra da unesete promjene na uređaju.
   3. U uređivaču registra dodajte vrijednost niza **SharedComputerLicensing** s postavkom 1 pod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na RDS poslužitelju ***prijavite se kao krajnji korisnik*** i provjerite je li [aktivacija dijeljenog računala omogućena za Microsoft 365 Apps za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

