---
title: Pitanja o korištenju alata za implementaciju sustava Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553532"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pitanja o korištenju alata za implementaciju sustava Office (ODT)

Preuzmite alat za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Nakon preuzimanja datoteke, pokrenite self-izdvajanje izvršne datoteke, koja sadrži Officeov alat implementacije izvršne (Setup. exe) i uzorak konfiguracijske datoteke (Configuration. xml).
  
 **Da biste isključili ili uklonili proizvode sustava Office 365 ProPlus s klijentskih računala:**
  
Prilikom instaliranja sustava Office 365 ProPlus možete izuzeti određene proizvode. Da biste to učinili, slijedite korake za instaliranje sustava Office s ODT-om, ali uključite element ExcludeApp u konfiguracijsku datoteku. Na primjer, ova konfiguracijska datoteka instalira sve proizvode sustava Office 365 ProPlus osim izdavača:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled alata za implementaciju sustava Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

