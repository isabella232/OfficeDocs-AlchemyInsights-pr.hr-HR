---
title: Korištenje alata za implementaciju sustava Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085824"
---
# <a name="using-the-office-deployment-tool-odt"></a>Korištenje alata za implementaciju sustava Office (ODT)

Pomoću alata za implementaciju sustava Office (ODT) možete implementirati verzije sustava Office 365 u sustavu Office. Alat za implementaciju sustava Office (setupodt.exe) pokreće se iz naredbenog retka i koristi konfiguracijsku XML datoteku da bi ustanovio koje se postavke primjenjuju pri implementaciji sustava Office.
  
1. Preuzmite najnoviju verziju alata za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Koristite [alat za prilagodbu sustava Office (Oct)](https://config.office.com) da biste odabrali svoje postavke implementacije i stvorili KONFIGURACIJSKU XML datoteku. Izvezite konfiguracijsku datoteku i postavite je lokalno na istu mapu u kojoj se nalazi setupodt.exe.

    **Upozorenje:** Problemi s instalacijom sustava Office obično se javljaju zbog pogrešnih konfiguriranih ili neoblikovanih konfiguracijskih datoteka. Da biste izbjegli takve probleme, preporučujemo da stvorite konfiguracijsku datoteku pomoću alata za prilagodbu sustava Office. Postojeće konfiguracijske datoteke možete uvesti i u alat za prilagodbu sustava Office.

3. Iz povišenog naredbenog upita prijeđite na mjesto na kojem setupodt.exe boravi i pokrenite alat za implementaciju sustava Office u načinu rada za preuzimanje i navedite konfiguracijsku datoteku koju ste upravo spremili. U ovom primjeru konfiguracijska datoteka naziva se Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. pokrenite alat za implementaciju sustava Office u modulu Konfiguriraj i navedite konfiguracijsku datoteku.

```setupodt.exe /configure Configuration.xml```

**Upozorenje:** Ovaj korak morate pokrenuti na klijentskom računalu na kojem želite instalirati Office, a na tom računalu morate imati lokalne administratorske dozvole.

Dodatne informacije o korištenju alata za implementaciju sustava Office za aplikacije Microsoft 365 za scenarije implementacije poduzeća potražite [u članku pregled alata za implementaciju sustava Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Dodatne informacije o korištenju alata za prilagodbu sustava Office potražite [u članku pregled alata za prilagodbu sustava Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
