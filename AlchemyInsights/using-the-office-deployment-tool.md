---
title: Korištenje alata za implementaciju sustava Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726240"
---
# <a name="using-the-office-deployment-tool-odt"></a>Korištenje alata za implementaciju sustava Office (ODT)

Koristite alat za implementaciju sustava Office (ODT) za implementaciju verzija sustava Office 365 sustava Office. Alat za implementaciju sustava Office (setup.exe) pokreće se iz naredbenog retka i koristi konfiguracijsku XML datoteku da bi odredio koje postavke primijeniti prilikom implementacije sustava Office.
  
1. Preuzmite najnoviju verziju alata za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Pomoću [alata za prilagodbu sustava Office (OCT)](https://config.office.com) odaberite postavke implementacije i stvorite konfiguracijsku XML datoteku. Izvezite konfiguracijsku datoteku i smjestite je lokalno u istu mapu u kojoj se nalazi setup.exe.

    **Napomena:** Problemi s instalacijom sustava Office obično nastaju zbog pogrešno konfiguriranih ili neoblikovanih konfiguracijskih datoteka. Da biste izbjegli takve probleme, preporučujemo da koristite alat za prilagodbu sustava Office za stvaranje konfiguracijske datoteke. Postojeće konfiguracijske datoteke možete uvesti i u alat za prilagodbu sustava Office.

3. From visok naredba brz, šiba to položaj gdje svisetup.exe preminka i trčanje Usluga Deployment Alat in preuzimanje datoteka način i specificirati oblik varalica te pravedan prišteđen. U ovom primjeru konfiguracijska datoteka se zove Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Pokrenite alat za implementaciju sustava Office u načinu konfiguriranja i odredite konfiguracijsku datoteku.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Napomena:** Ovaj korak morate pokrenuti s klijentskog računala na koje želite instalirati Office i morate imati dozvole lokalnog administratora na tom računalu.

Dodatne informacije o korištenju alata za implementaciju sustava Office za scenarije implementacije sustava Microsoft 365 za tvrtke potražite [u članku Pregled alata za implementaciju sustava Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Dodatne informacije o korištenju alata za prilagodbu sustava Office potražite u članku [Pregled alata za prilagodbu sustava Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
