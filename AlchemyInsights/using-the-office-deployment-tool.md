---
title: Korištenje alata Office implementacije
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083762"
---
# <a name="using-the-office-deployment-tool-odt"></a>Korištenje alata Office implementacije (ODT)

Koristite alat za Office implementaciju (ODT) za implementaciju Office 365 verzija Office. Alat Office implementacije (setup.exe) pokrenuti će se iz naredbenog retka i koristi konfiguracijsku XML datoteku da bi se utvrdilo koje se postavke primjenjuju prilikom implementacije Office.
  
1. Preuzmite najnoviju verziju alata za implementaciju Office iz Microsoftova [centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Pomoću [alata Office prilagodbe (OCT)](https://config.office.com) odaberite postavke implementacije i stvorite konfiguracijsku XML datoteku. Izvezite konfiguracijsku datoteku i postavite je lokalno u istu mapu u kojoj setup.exe nalazi.

    **Napomena:** Office se problemi s instalacijom najčešće pojavljuju zbog pogrešno konfiguriranih ili pogrešno oblikovanih konfiguracijskih datoteka. Da biste izbjegli takve probleme, preporučujemo da pomoću alata za Office za prilagodbu stvorite konfiguracijsku datoteku. Postojeće konfiguracijske datoteke možete uvesti i u alat za Office prilagodbe.

3. Iz povišenog naredbenog retka prijeđite na mjesto na kojem se setup.exe nalazi i pokrenite alat za implementaciju Office u načinu rada za preuzimanje i navedite konfiguracijsku datoteku koju ste upravo spremili. U ovom se primjeru konfiguracijska datoteka naziva Configuration.xml:

```setup.exe /download Configuration.xml```

4.Pokrenite alat Office implementacije u načinu konfiguriranja i odredite konfiguracijsku datoteku.

```setup.exe /configure Configuration.xml```

**Napomena:** Taj korak morate pokrenuti s klijentskog računala na koje želite instalirati Office morate imati dozvole lokalnog administratora na tom računalu.

Dodatne informacije o korištenju alata Office implementacije za scenarije implementacije sustava Microsoft 365 Apps za velike tvrtke potražite u [članku Pregled alata Office implementacije](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Dodatne informacije o tome kako koristiti alat za Office prilagodbe potražite u [članku Pregled alata za Office prilagodbe](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
