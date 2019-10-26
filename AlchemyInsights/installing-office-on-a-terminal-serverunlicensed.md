---
title: Instaliranje ureda na terminalskom poslužitelju-Nelicencirano
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/25/2019
ms.locfileid: "37205401"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="3c3f2-102">Instaliranje Officea na terminalskom poslužitelju</span><span class="sxs-lookup"><span data-stu-id="3c3f2-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="3c3f2-103">Za uvođenje sustava Office 365 ProPlus na Windows Server pomoću usluga udaljene radne površine (RDS), ranije imena Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="3c3f2-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="3c3f2-104">Morate imati Office 365 plan koji uključuje Office 365 ProPlus, kao što su Office 365 Enterprise E3 ili Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="3c3f2-105">Planovi Office 365 Business i Office 365 Business Premium ne uključuju Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="3c3f2-106">Morate omogućiti [aktivaciju zajedničkog računala](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="3c3f2-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="3c3f2-107">Ako želite instalirati Office 365 ProPlus na RDS iz centra Microsoft 365 admin, ***koji koristi zadane instalacije postavke***, koristite sljedeće korake.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="3c3f2-108">Također možete preuzeti i pokrenuti [Microsoftov pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) da biste instalirali Office 365 proplus u načinu rada za aktivaciju zajedničkog računala.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="3c3f2-109">Provjerite koji Office 365 plan imate.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="3c3f2-110">Naučite kako</span><span class="sxs-lookup"><span data-stu-id="3c3f2-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="3c3f2-111">Ako je potrebno, prebacite se na drugi Office 365 plan.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="3c3f2-112">Naučite kako</span><span class="sxs-lookup"><span data-stu-id="3c3f2-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="3c3f2-113">Ako je Office već instaliran na poslužitelju RDS pomoću bilo kojeg drugog Office 365 planova, deinstalirati ga.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="3c3f2-114">Na primjer, ako idete na Upravljačka ploča \> deinstalirati program.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="3c3f2-115">Deinstalirajte pomoću [Microsoftove podrške i oporavka od pomoćnika](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako ste u problemima.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="3c3f2-116">Na RDS poslužitelju, prijavite se na Microsoft 365 Admin Center s administratorskim računom i [instalirajte Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="3c3f2-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="3c3f2-117">Nakon instalacije sustava Office ***Nemojte otvarati ili se prijaviti u*** bilo koje aplikacije sustava Office.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="3c3f2-118">Na RDS poslužitelju omogućite zajedničko računalo aktivaciju uređivanjem registra slijedeći ove korake:</span><span class="sxs-lookup"><span data-stu-id="3c3f2-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="3c3f2-119">Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite Pokreni.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="3c3f2-120">U okvir Otvori upišite **regedit**, a zatim odaberite u redu.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="3c3f2-121">Odaberite da kada se od vas zatraži da omogućite uređivač registra da napravi promjene na uređaju.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="3c3f2-122">U uređivač registra dodajte vrijednost niza **Sharedcomputer,** uz postavku 1 ispod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="3c3f2-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="3c3f2-123">Na RDS poslužitelju prijavite se ***kao krajnji korisnik*** i [Provjerite je li aktivacija zajedničkog računala omogućena za Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="3c3f2-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="3c3f2-124">Za više detalja o preduvjeta, upute za postavljanje i smjernice o prilagođenim instalacijama pomoću alata za implementaciju sustava Office potražite u [instalaciji sustava office 365 ProPlus pomoću usluga udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="3c3f2-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="3c3f2-125">Da biste riješili pogreške povezane s aktivacijom zajedničkog računala, pogledajte [Rješavanje problema s aktivacijom zajedničkog računala za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="3c3f2-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  