---
title: Pitanja o tome kako koristiti alat za Office implementaciju (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959675"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pitanja o tome kako koristiti alat za Office implementaciju (ODT)

Preuzmite alat Office implementacije iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Nakon preuzimanja datoteke pokrenite izvršnu datoteku koja se sama izdvaja, koja sadrži izvršnu datoteku alata Office implementacije (setup.exe) i oglednu konfiguracijsku datoteku (configuration.xml).
  
 **Da biste izuzeli ili uklonili Microsoft 365 Apps za velike tvrtke s klijentskih računala:**
  
Prilikom instalacije Microsoft 365 Apps za velike tvrtke, možete izuzeti određene proizvode. Da biste to učiniti, slijedite korake za Office instalaciju pomoću ODT-a, ali u konfiguracijsku datoteku uvrstite element ExcludeApp. Na primjer, ova konfiguracijska datoteka instalira sve Microsoft 365 Apps za velike tvrtke proizvode osim Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled alata Office implementacije](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

