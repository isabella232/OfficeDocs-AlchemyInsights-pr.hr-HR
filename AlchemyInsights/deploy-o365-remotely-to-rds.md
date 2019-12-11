---
title: Implementacija Office 365 ProPlus za zajedničko korištenje na RDS, Terminal Server, ili VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959452"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="96d0a-102">Implementacija Office 365 ProPlus za zajedničko korištenje na RDS, Terminal Server, ili VDI</span><span class="sxs-lookup"><span data-stu-id="96d0a-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="96d0a-103">Da biste implementirati Office 365 ProPlus pomoću usluga udaljene radne površine (RDS), ranije imena Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="96d0a-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="96d0a-104">Morate imati Microsoft 365 za Business plan ili Office 365 plan koji uključuje Office 365 ProPlus, kao što su Office 365 Enterprise E3 ili Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="96d0a-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="96d0a-105">Planovi Office 365 Business i Office 365 Business Premium ne uključuju Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="96d0a-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="96d0a-106">Morate omogućiti [aktivaciju zajedničkog računala](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="96d0a-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="96d0a-107">Također možete preuzeti i pokrenuti [Microsoftov pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) da biste instalirali Office 365 proplus u načinu rada za aktivaciju zajedničkog računala.</span><span class="sxs-lookup"><span data-stu-id="96d0a-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="96d0a-108">Dodatne informacije o preduvjete, uputama za postavljanje i smjernicama o prilagođenim instalacijama pomoću alata za implementaciju sustava Office potražite u uputi [office 365 ProPlus pomoću usluga udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="96d0a-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="96d0a-109">Da biste riješili pogreške povezane s aktivacijom zajedničkog računala:</span><span class="sxs-lookup"><span data-stu-id="96d0a-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="96d0a-110">Pogledajte [Rješavanje problema s aktivacijom zajedničkog računala za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="96d0a-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="96d0a-111">Pogledajte [reset Office 365 ProPlus stanje aktivacije](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="96d0a-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="96d0a-112">Ako želite instalirati Office 365 ProPlus na RDS iz centra Microsoft 365 admin, ***koji koristi zadane instalacije postavke***, koristite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="96d0a-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="96d0a-113">Provjerite koji Office 365 plan imate.</span><span class="sxs-lookup"><span data-stu-id="96d0a-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="96d0a-114">[Nauči kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="96d0a-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="96d0a-115">Ako je potrebno, prebacite se na drugi Office 365 plan.</span><span class="sxs-lookup"><span data-stu-id="96d0a-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="96d0a-116">[Nauči kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="96d0a-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="96d0a-117">Ako je Office već instaliran na poslužitelju RDS pomoću bilo kojeg drugog Office 365 planova, deinstalirati ga.</span><span class="sxs-lookup"><span data-stu-id="96d0a-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="96d0a-118">Na primjer, idete na **upravljačku ploču** > **deinstalirati program**.</span><span class="sxs-lookup"><span data-stu-id="96d0a-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="96d0a-119">Deinstalirajte pomoću [Microsoftove podrške i oporavka od pomoćnika](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako ste u problemima.</span><span class="sxs-lookup"><span data-stu-id="96d0a-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="96d0a-120">Na RDS poslužitelju, prijavite se na Microsoft 365 Admin Center s administratorskim računom i [instalirajte Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="96d0a-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="96d0a-121">Nakon instalacije sustava Office ***Nemojte otvarati ili se prijaviti u*** bilo koje aplikacije sustava Office.</span><span class="sxs-lookup"><span data-stu-id="96d0a-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="96d0a-122">Na RDS poslužitelju omogućite zajedničko računalo aktivaciju uređivanjem registra slijedeći ove korake:</span><span class="sxs-lookup"><span data-stu-id="96d0a-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="96d0a-123">Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite **Pokreni**.</span><span class="sxs-lookup"><span data-stu-id="96d0a-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="96d0a-124">U okvir Otvori upišite **regedit**, a zatim odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="96d0a-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="96d0a-125">Odaberite **da** kada se od vas zatraži da omogućite uređivač registra da napravi promjene na uređaju.</span><span class="sxs-lookup"><span data-stu-id="96d0a-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="96d0a-126">U uređivaču registra dodajte vrijednost niza **Sharedcomputer,** uz postavku 1 u odjeljku HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="96d0a-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="96d0a-127">Na RDS poslužitelju prijavite se ***kao krajnji korisnik*** i [Provjerite je li aktivacija zajedničkog računala omogućena za Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="96d0a-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

