---
title: Pomoću alata za uvođenje Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365517"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="6c3a9-102">Pomoću alata za uvođenje Office (odt-a)</span><span class="sxs-lookup"><span data-stu-id="6c3a9-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="6c3a9-103">Koristite u Office Deployment alat (odt-a) za uvođenje Office 365 verzijama paketa Office.</span><span class="sxs-lookup"><span data-stu-id="6c3a9-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="6c3a9-104">Alat za implementaciju paketa Office (setup.exe) je pokrenuti iz naredbenog retka i koristi XML datoteku za konfiguraciju da biste odredili koje će se postavke primijeniti pri implementaciji sustava Office.</span><span class="sxs-lookup"><span data-stu-id="6c3a9-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="6c3a9-105">Iz [Microsoftova centra za preuzimanje](http://go.microsoft.com/fwlink/p/?LinkID=626065)preuzmite najnoviju verziju alata uvođenja paketa Office.</span><span class="sxs-lookup"><span data-stu-id="6c3a9-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="6c3a9-106">Koristite [Alat za prilagodbu Office (lis)](https://config.office.com) odaberite preference uvođenja i stvoriti konfiguracijsku datoteku XML.</span><span class="sxs-lookup"><span data-stu-id="6c3a9-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="6c3a9-107">Izvoz konfiguracijske datoteke i stavite ga lokalno na istu mapu gdje se nalazi setup.exe.</span><span class="sxs-lookup"><span data-stu-id="6c3a9-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="6c3a9-108">**Napomena:** Instalacija programa Office problemi najčešće pojavljuju dospijeća za misconfigured ili malformatted konfiguracijske datoteke.</span><span class="sxs-lookup"><span data-stu-id="6c3a9-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="6c3a9-109">Da biste izbjegli takve probleme, preporučujemo da koristite alat za prilagodbu Office za stvaranje konfiguracijske datoteke.</span><span class="sxs-lookup"><span data-stu-id="6c3a9-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="6c3a9-110">Postojeće konfiguracijske datoteke možete uvesti i u alat za prilagodbu Office.</span><span class="sxs-lookup"><span data-stu-id="6c3a9-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="6c3a9-111">Iz privilegiranom naredbenom retku prijeđite na mjesto gdje se nalazi setup.exe i pokretanje alata za uvođenje Office u načinu preuzimanja i navedite konfiguracijsku datoteku koju ste upravo spremili.</span><span class="sxs-lookup"><span data-stu-id="6c3a9-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="6c3a9-112">U ovom primjeru konfiguracijsku datoteku pod nazivom Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="6c3a9-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="6c3a9-113">Pokrenite alat za implementaciju paketa Office u konfigurirajte način i navedite konfiguracijsku datoteku.</span><span class="sxs-lookup"><span data-stu-id="6c3a9-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="6c3a9-114">**Napomena:** Ovaj korak morate pokrenuti s klijentskog računala na koji želite instalirati Office i morate imati dozvole za lokalni administrator na tom računalu.</span><span class="sxs-lookup"><span data-stu-id="6c3a9-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="6c3a9-115">Da biste saznali više o korištenju alata za uvođenje Office za Office 365 ProPlus scenarije uvođenja, pogledajte [Pregled alat za implementaciju paketa Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="6c3a9-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="6c3a9-116">Za dodatne pojedinosti o tome kako koristiti alat za prilagodbu Office pogledajte [Pregled alat za prilagodbu Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="6c3a9-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
