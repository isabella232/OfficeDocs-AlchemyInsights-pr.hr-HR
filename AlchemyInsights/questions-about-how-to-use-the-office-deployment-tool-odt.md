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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="a540b-102">Pitanja o korištenju alata za implementaciju sustava Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="a540b-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="a540b-103">Preuzmite alat za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="a540b-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="a540b-104">Nakon preuzimanja datoteke pokrenite izvršnu datoteku koja se sama izdvaja, koja sadrži izvršnu datoteku alata za implementaciju sustava Office (setup.exe) i oglednu konfiguracijsku datoteku (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="a540b-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="a540b-105">**Da biste izuzeli ili uklonili Aplikacije sustava Microsoft 365 za poslovne proizvode s klijentskih računala:**</span><span class="sxs-lookup"><span data-stu-id="a540b-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="a540b-106">Prilikom instalacije aplikacija microsoft 365 za tvrtke možete izuzeti određene proizvode.</span><span class="sxs-lookup"><span data-stu-id="a540b-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="a540b-107">Da biste to učinili, slijedite korake za instalaciju sustava Office s ODT-om, ali u konfiguracijsku datoteku uključite element ExcludeApp.</span><span class="sxs-lookup"><span data-stu-id="a540b-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="a540b-108">Na primjer, ova konfiguracijska datoteka instalira sve Aplikacije sustava Microsoft 365 za poslovne proizvode osim programa Publisher:</span><span class="sxs-lookup"><span data-stu-id="a540b-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="a540b-109">Pregled alata za implementaciju sustava Office</span><span class="sxs-lookup"><span data-stu-id="a540b-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

