---
title: Korištenje alata za implementaciju sustava Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085824"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="ca7c2-102">Korištenje alata za implementaciju sustava Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="ca7c2-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="ca7c2-103">Pomoću alata za implementaciju sustava Office (ODT) možete implementirati verzije sustava Office 365 u sustavu Office.</span><span class="sxs-lookup"><span data-stu-id="ca7c2-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="ca7c2-104">Alat za implementaciju sustava Office (setupodt.exe) pokreće se iz naredbenog retka i koristi konfiguracijsku XML datoteku da bi ustanovio koje se postavke primjenjuju pri implementaciji sustava Office.</span><span class="sxs-lookup"><span data-stu-id="ca7c2-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="ca7c2-105">Preuzmite najnoviju verziju alata za implementaciju sustava Office iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="ca7c2-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="ca7c2-106">Koristite [alat za prilagodbu sustava Office (Oct)](https://config.office.com) da biste odabrali svoje postavke implementacije i stvorili KONFIGURACIJSKU XML datoteku.</span><span class="sxs-lookup"><span data-stu-id="ca7c2-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="ca7c2-107">Izvezite konfiguracijsku datoteku i postavite je lokalno na istu mapu u kojoj se nalazi setupodt.exe.</span><span class="sxs-lookup"><span data-stu-id="ca7c2-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="ca7c2-108">**Upozorenje:** Problemi s instalacijom sustava Office obično se javljaju zbog pogrešnih konfiguriranih ili neoblikovanih konfiguracijskih datoteka.</span><span class="sxs-lookup"><span data-stu-id="ca7c2-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="ca7c2-109">Da biste izbjegli takve probleme, preporučujemo da stvorite konfiguracijsku datoteku pomoću alata za prilagodbu sustava Office.</span><span class="sxs-lookup"><span data-stu-id="ca7c2-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="ca7c2-110">Postojeće konfiguracijske datoteke možete uvesti i u alat za prilagodbu sustava Office.</span><span class="sxs-lookup"><span data-stu-id="ca7c2-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="ca7c2-111">Iz povišenog naredbenog upita prijeđite na mjesto na kojem setupodt.exe boravi i pokrenite alat za implementaciju sustava Office u načinu rada za preuzimanje i navedite konfiguracijsku datoteku koju ste upravo spremili.</span><span class="sxs-lookup"><span data-stu-id="ca7c2-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="ca7c2-112">U ovom primjeru konfiguracijska datoteka naziva se Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="ca7c2-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="ca7c2-113">4. pokrenite alat za implementaciju sustava Office u modulu Konfiguriraj i navedite konfiguracijsku datoteku.</span><span class="sxs-lookup"><span data-stu-id="ca7c2-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="ca7c2-114">**Upozorenje:** Ovaj korak morate pokrenuti na klijentskom računalu na kojem želite instalirati Office, a na tom računalu morate imati lokalne administratorske dozvole.</span><span class="sxs-lookup"><span data-stu-id="ca7c2-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="ca7c2-115">Dodatne informacije o korištenju alata za implementaciju sustava Office za aplikacije Microsoft 365 za scenarije implementacije poduzeća potražite [u članku pregled alata za implementaciju sustava Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="ca7c2-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="ca7c2-116">Dodatne informacije o korištenju alata za prilagodbu sustava Office potražite [u članku pregled alata za prilagodbu sustava Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="ca7c2-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
