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
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774883"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="6f637-102">Pitanja o korištenju alata za implementaciju sustava Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="6f637-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="6f637-103">Preuzmite alat za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="6f637-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="6f637-104">Kada preuzmete datoteku, pokrenite samoizdvajanje izvršnu datoteku koja sadrži izvršne alate za implementaciju sustava Office (setup.exe) te oglednu konfiguracijsku datoteku (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="6f637-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="6f637-105">**Da biste isključili ili uklonili aplikacije Microsoft 365 za Enterprise Products sa klijentskih računala, učinite sljedeće:**</span><span class="sxs-lookup"><span data-stu-id="6f637-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="6f637-106">Prilikom instalacije aplikacija Microsoft 365 za Enterprise možete isključiti specifične proizvode.</span><span class="sxs-lookup"><span data-stu-id="6f637-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="6f637-107">Da biste to učinili, slijedite korake za instaliranje sustava Office s ODT-om, ali u konfiguracijskoj datoteci uvrstite element ExcludeApp.</span><span class="sxs-lookup"><span data-stu-id="6f637-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="6f637-108">Ta konfiguracijska datoteka, primjerice, instalira sve aplikacije Microsoft 365 za tvrtke, osim programa Publisher:</span><span class="sxs-lookup"><span data-stu-id="6f637-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="6f637-109">Pregled alata za implementaciju sustava Office</span><span class="sxs-lookup"><span data-stu-id="6f637-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

