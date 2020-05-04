---
title: Korištenje alata za implementaciju sustava Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010849"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="35a80-102">Korištenje alata za implementaciju sustava Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="35a80-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="35a80-103">Koristite alat za implementaciju sustava Office (ODT) za implementaciju verzija sustava Office 365 sustava Office.</span><span class="sxs-lookup"><span data-stu-id="35a80-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="35a80-104">Alat za implementaciju sustava Office (setup.exe) pokreće se iz naredbenog retka i koristi konfiguracijsku XML datoteku da bi odredio koje postavke primijeniti prilikom implementacije sustava Office.</span><span class="sxs-lookup"><span data-stu-id="35a80-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="35a80-105">Preuzmite najnoviju verziju alata za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="35a80-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="35a80-106">Pomoću [alata za prilagodbu sustava Office (OCT)](https://config.office.com) odaberite postavke implementacije i stvorite konfiguracijsku XML datoteku.</span><span class="sxs-lookup"><span data-stu-id="35a80-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="35a80-107">Izvezite konfiguracijsku datoteku i smjestite je lokalno u istu mapu u kojoj se nalazi setup.exe.</span><span class="sxs-lookup"><span data-stu-id="35a80-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="35a80-108">**Napomena:** Problemi s instalacijom sustava Office obično nastaju zbog pogrešno konfiguriranih ili neoblikovanih konfiguracijskih datoteka.</span><span class="sxs-lookup"><span data-stu-id="35a80-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="35a80-109">Da biste izbjegli takve probleme, preporučujemo da koristite alat za prilagodbu sustava Office za stvaranje konfiguracijske datoteke.</span><span class="sxs-lookup"><span data-stu-id="35a80-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="35a80-110">Postojeće konfiguracijske datoteke možete uvesti i u alat za prilagodbu sustava Office.</span><span class="sxs-lookup"><span data-stu-id="35a80-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="35a80-111">From visok naredba brz, šiba to položaj gdje svisetup.exe preminka i trčanje Usluga Deployment Alat in preuzimanje datoteka način i specificirati oblik varalica te pravedan prišteđen.</span><span class="sxs-lookup"><span data-stu-id="35a80-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="35a80-112">U ovom primjeru konfiguracijska datoteka se zove Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="35a80-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="35a80-113">Pokrenite alat za implementaciju sustava Office u načinu konfiguriranja i odredite konfiguracijsku datoteku.</span><span class="sxs-lookup"><span data-stu-id="35a80-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="35a80-114">**Napomena:** Ovaj korak morate pokrenuti s klijentskog računala na koje želite instalirati Office i morate imati dozvole lokalnog administratora na tom računalu.</span><span class="sxs-lookup"><span data-stu-id="35a80-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="35a80-115">Dodatne informacije o korištenju alata za implementaciju sustava Office za scenarije implementacije sustava Microsoft 365 za tvrtke potražite [u članku Pregled alata za implementaciju sustava Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="35a80-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="35a80-116">Dodatne informacije o korištenju alata za prilagodbu sustava Office potražite u članku [Pregled alata za prilagodbu sustava Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="35a80-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
