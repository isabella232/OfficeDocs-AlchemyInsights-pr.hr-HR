---
title: Pitanja o tome kako koristiti alat za implementaciju sustava Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790324"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pitanja o tome kako koristiti alat za implementaciju sustava Office (ODT)

Preuzmite alat za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Nakon preuzimanja datoteke pokrenite samostalnu izvršnu datoteku koja sadrži izvršnu datoteku alata za implementaciju sustava Office (setup.exe) i oglednu konfiguracijsku datoteku (configuration.xml).
  
 **Da biste izuzeli ili uklonili aplikacije Microsoft 365 za korporacijske proizvode s klijentskih računala:**
  
Prilikom instalacije aplikacija Microsoft 365 za velike tvrtke možete izuzeti određene proizvode. Da biste to učiniti, slijedite korake za instalaciju sustava Office pomoću ODT-a, ali u konfiguracijsku datoteku uvrstite element ExcludeApp. Na primjer, ova konfiguracijska datoteka instalira sve aplikacije sustava Microsoft 365 za poslovne proizvode osim programa Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled alata za implementaciju sustava Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

