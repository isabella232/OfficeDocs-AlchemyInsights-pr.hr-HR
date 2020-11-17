---
title: Pitanja o korištenju alata za implementaciju sustava Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086148"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pitanja o korištenju alata za implementaciju sustava Office (ODT)

Preuzmite alat za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Kada preuzmete datoteku, pokrenite samoizdvajanje izvršnu datoteku koja sadrži izvršne alate za implementaciju sustava Office (setupodt.exe) te oglednu konfiguracijsku datoteku (configuration.xml).
  
 **Da biste isključili ili uklonili aplikacije Microsoft 365 za Enterprise Products sa klijentskih računala, učinite sljedeće:**
  
Prilikom instalacije aplikacija Microsoft 365 za Enterprise možete isključiti specifične proizvode. Da biste to učinili, slijedite korake za instaliranje sustava Office s ODT-om, ali u konfiguracijskoj datoteci uvrstite element ExcludeApp. Ta konfiguracijska datoteka, primjerice, instalira sve aplikacije Microsoft 365 za tvrtke, osim programa Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled alata za implementaciju sustava Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

