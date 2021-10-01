---
title: Implementacija Microsoft 365 Apps za zajedničko korištenje na servisima RDS, Terminal Server ili VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077242"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementacija Microsoft 365 Apps za zajedničko korištenje na servisima RDS, Terminal Server ili VDI

Da biste Microsoft 365 Apps servise udaljene radne površine (RDS), prije servisa Terminal Services, morate:

- Pomoću jednostavnog popravka omogućite TLS 1.2 kao zadano ako koristite stariju verziju sustava Windows (npr. Windows 7 SP1, Windows Server 2008 R2). Da biste jednostavno ispravili i dodatne informacije, pogledajte ažuriranje da biste [omogućili TLS 1.1 i TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)kao zadane sigurne protokole u sustavu WinHTTP u Windows . 
- Imati plan koji sadrži Microsoft 365 Apps za velike tvrtke (prethodno Office 365 Plus). Na primjer, Office 365 E3 ili Microsoft 365 E5 ili bilo koji plan koji obuhvaća verziju programa Project ili Visio za stolna računala, kao što su Project tarifa 3 ili Visio tarifa 2, ili Microsoft 365 Business Premium plan, koji obuhvaća i Microsoft 365 Apps za male tvrtke.
- Omogućivanje aktivacije zajedničkog računala. Dodatne informacije potražite u članku Pregled [aktivacije zajedničkog računala za Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Napomena:** da biste Microsoft 365 Apps u načinu aktivacije zajedničkog računala, preuzmite i pokrenite [Microsoft pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal). Detalje o preduvjetima, uputama za postavljanje i uputama za prilagodbu instalacija pomoću alata za implementaciju Office potražite u [članku Implementacija Microsoft 365 Apps korištenjem](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)servisa udaljene radne površine .

Da biste ispravili pogreške povezane s aktivacijom zajedničkog računala, pogledajte sljedeće:

- [Otklanjanje poteškoća s aktivacijom zajedničkog računala za Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Ponovno Microsoft 365 Apps za velike tvrtke stanje aktivacije](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Ako želite instalirati Microsoft 365 Apps RDS iz Centar za administratore okruženja Microsoft 365, koji koristi zadane postavke instalacije, slijedite ove korake:

1. Provjerite koji Microsoft 365 plan imate. Dodatne informacije potražite u [članku Koju pretplatu imam?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Ako je potrebno, prijeđite na drugu Microsoft 365 plan. Dodatne informacije potražite u članku [Nadogradnja na drugu plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Ako Microsoft 365 Apps već instaliran na RDS poslužitelju pomoću bilo koje druge nekompatibilne tarife, deinstalirajte ga tako da ode na **Upravljačka**  >  **ploča Deinstaliranje programa**. Ako naiđete na probleme, deinstalirajte tako da [preuzmete Microsoft pomoćnik za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. Na RDS poslužitelju prijavite se na Centar za administratore okruženja Microsoft 365 pomoću administratorskog računa i [instalirajte Office](https://portal.office.com/OLS/MySoftware.aspx).

   Kada Office instalirate, nemojte se otvarati ni prijaviti u bilo koju Office aplikacije.

1. Na RDS poslužitelju omogućite aktivaciju zajedničkog računala uređivanjem registra:

   1. Desnom tipkom miša kliknite Windows u donjem lijevom kutu zaslona pa odaberite **Pokreni**. U okvir Otvori upišite **regedit**, a zatim odaberite U **redu**.

   1. Kada se od vas zatraži da omogućite uređivaču registra da unosi promjene na uređaj, odaberite **Da**.

   1. U uređivaču registra u odjeljku HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration dodajte vrijednost niza **za SharedComputerLicensing** s postavkom **1** .

1. Na RDS poslužitelju prijavite se kao krajnji korisnik i provjerite je li omogućena aktivacija zajedničkog računala za Microsoft 365 Apps. 

   Detalje potražite u članku [Provjera je li omogućena aktivacija zajedničkog računala za Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).