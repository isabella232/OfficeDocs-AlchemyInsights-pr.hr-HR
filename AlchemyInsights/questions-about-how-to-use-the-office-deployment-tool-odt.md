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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="31ad5-102">Pitanja o korištenju alata za implementaciju sustava Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="31ad5-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="31ad5-103">Preuzmite alat za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="31ad5-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="31ad5-104">Kada preuzmete datoteku, pokrenite samoizdvajanje izvršnu datoteku koja sadrži izvršne alate za implementaciju sustava Office (setupodt.exe) te oglednu konfiguracijsku datoteku (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="31ad5-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="31ad5-105">**Da biste isključili ili uklonili aplikacije Microsoft 365 za Enterprise Products sa klijentskih računala, učinite sljedeće:**</span><span class="sxs-lookup"><span data-stu-id="31ad5-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="31ad5-106">Prilikom instalacije aplikacija Microsoft 365 za Enterprise možete isključiti specifične proizvode.</span><span class="sxs-lookup"><span data-stu-id="31ad5-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="31ad5-107">Da biste to učinili, slijedite korake za instaliranje sustava Office s ODT-om, ali u konfiguracijskoj datoteci uvrstite element ExcludeApp.</span><span class="sxs-lookup"><span data-stu-id="31ad5-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="31ad5-108">Ta konfiguracijska datoteka, primjerice, instalira sve aplikacije Microsoft 365 za tvrtke, osim programa Publisher:</span><span class="sxs-lookup"><span data-stu-id="31ad5-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="31ad5-109">Pregled alata za implementaciju sustava Office</span><span class="sxs-lookup"><span data-stu-id="31ad5-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

