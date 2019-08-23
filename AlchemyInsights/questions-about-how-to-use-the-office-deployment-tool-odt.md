---
title: Pitanja kako koristiti u Office Deployment alat (odt-a)
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553532"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pitanja kako koristiti u Office Deployment alat (odt-a)

Iz [Microsoftova centra za preuzimanje](http://go.microsoft.com/fwlink/p/?LinkID=626065)Preuzmite alat za implementaciju paketa Office.
  
Nakon preuzimanja datoteke, pokrenite samoizdvojiva izvršna datoteka, koje sadrži Office Deployment alat izvršne (setup.exe) i uzorak konfiguracijska datoteka (configuration.xml).
  
 **Isključi ili ukloniti Office 365 ProPlus proizvode iz klijentskih računala:**
  
Kada instalirate Office 365 ProPlus, možete isključiti određene proizvode. Da biste to učinili, slijedite korake za instalaciju Office s u odt-a, ali uključiti ExcludeApp element u konfiguracijskoj datoteci. Na primjer, konfiguracijska datoteka instalira Office 365 ProPlus proizvode osim programa Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled alata za uvođenje Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

