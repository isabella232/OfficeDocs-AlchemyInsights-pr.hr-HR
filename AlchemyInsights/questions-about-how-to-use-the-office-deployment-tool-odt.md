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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="48c72-102">Pitanja o korištenju alata za implementaciju sustava Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="48c72-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="48c72-103">Preuzmite alat za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="48c72-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="48c72-104">Nakon preuzimanja datoteke, pokrenite self-izdvajanje izvršne datoteke, koja sadrži Officeov alat implementacije izvršne (Setup. exe) i uzorak konfiguracijske datoteke (Configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="48c72-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="48c72-105">**Da biste isključili ili uklonili proizvode sustava Office 365 ProPlus s klijentskih računala:**</span><span class="sxs-lookup"><span data-stu-id="48c72-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="48c72-106">Prilikom instaliranja sustava Office 365 ProPlus možete izuzeti određene proizvode.</span><span class="sxs-lookup"><span data-stu-id="48c72-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="48c72-107">Da biste to učinili, slijedite korake za instaliranje sustava Office s ODT-om, ali uključite element ExcludeApp u konfiguracijsku datoteku.</span><span class="sxs-lookup"><span data-stu-id="48c72-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="48c72-108">Na primjer, ova konfiguracijska datoteka instalira sve proizvode sustava Office 365 ProPlus osim izdavača:</span><span class="sxs-lookup"><span data-stu-id="48c72-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="48c72-109">Pregled alata za implementaciju sustava Office</span><span class="sxs-lookup"><span data-stu-id="48c72-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

