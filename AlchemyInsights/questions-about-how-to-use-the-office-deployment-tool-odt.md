---
title: Pitanja o korištenju alata za implementaciju sustava Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010723"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pitanja o korištenju alata za implementaciju sustava Office (ODT)

Preuzmite alat za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Nakon preuzimanja datoteke pokrenite izvršnu datoteku koja se sama izdvaja, koja sadrži izvršnu datoteku alata za implementaciju sustava Office (setup.exe) i oglednu konfiguracijsku datoteku (configuration.xml).
  
 **Da biste izuzeli ili uklonili Aplikacije sustava Microsoft 365 za poslovne proizvode s klijentskih računala:**
  
Prilikom instalacije aplikacija microsoft 365 za tvrtke možete izuzeti određene proizvode. Da biste to učinili, slijedite korake za instalaciju sustava Office s ODT-om, ali u konfiguracijsku datoteku uključite element ExcludeApp. Na primjer, ova konfiguracijska datoteka instalira sve Aplikacije sustava Microsoft 365 za poslovne proizvode osim programa Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled alata za implementaciju sustava Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

