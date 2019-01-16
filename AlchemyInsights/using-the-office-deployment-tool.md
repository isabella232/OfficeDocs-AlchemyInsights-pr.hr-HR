---
title: Pomoću alata za uvođenje Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28280418"
---
# <a name="using-the-office-deployment-tool-odt"></a>Pomoću alata za uvođenje Office (odt-a)

Koristite u Office Deployment alat (odt-a) za uvođenje Office 365 verzijama paketa Office. Alat za implementaciju paketa Office (setup.exe) je pokrenuti iz naredbenog retka i koristi XML datoteku za konfiguraciju da biste odredili koje će se postavke primijeniti pri implementaciji sustava Office.
  
1. Iz [Microsoftova centra za preuzimanje](http://go.microsoft.com/fwlink/p/?LinkID=626065)preuzmite najnoviju verziju alata uvođenja paketa Office.
    
2. Koristite [Alat za prilagodbu Office (lis)](https://config.office.com) odaberite preference uvođenja i stvoriti konfiguracijsku datoteku XML. Izvoz konfiguracijske datoteke i stavite ga lokalno na istu mapu gdje se nalazi setup.exe. 
    
    **Napomena:** Instalacija programa Office problemi najčešće pojavljuju dospijeća za misconfigured ili malformatted konfiguracijske datoteke. Da biste izbjegli takve probleme, preporučujemo da koristite alat za prilagodbu Office za stvaranje konfiguracijske datoteke. Postojeće konfiguracijske datoteke možete uvesti i u alat za prilagodbu Office. 
    
3. Iz privilegiranom naredbenom retku prijeđite na mjesto gdje se nalazi setup.exe i pokretanje alata za uvođenje Office u načinu preuzimanja i navedite konfiguracijsku datoteku koju ste upravo spremili. U ovom primjeru konfiguracijsku datoteku pod nazivom Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Pokrenite alat za implementaciju paketa Office u konfigurirajte način i navedite konfiguracijsku datoteku.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Napomena:** Ovaj korak morate pokrenuti s klijentskog računala na koji želite instalirati Office i morate imati dozvole za lokalni administrator na tom računalu. 
    
Da biste saznali više o korištenju alata za uvođenje Office za Office 365 ProPlus scenarije uvođenja, pogledajte [Pregled alat za implementaciju paketa Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Za dodatne pojedinosti o tome kako koristiti alat za prilagodbu Office pogledajte [Pregled alat za prilagodbu Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

