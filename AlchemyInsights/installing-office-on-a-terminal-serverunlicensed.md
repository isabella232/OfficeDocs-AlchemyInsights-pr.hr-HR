---
title: Instaliranje sustava office na Terminal Serveru - nelicenciran
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: edac051840594f13b22ccd83f5cd6e3da5f84cbc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36498407"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="44f64-102">Instaliranje sustava Office na terminalski poslužitelj</span><span class="sxs-lookup"><span data-stu-id="44f64-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="44f64-103">Za uvođenje Office 365 ProPlus na poslužitelju Windows pomoću udaljene radne površine Services (ZAPISI), prije naziva servisa Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="44f64-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="44f64-104">Morate imati Office 365 plan koji uključuje Office 365 ProPlus, kao što je Office 365 Enterprise E3 ili Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="44f64-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="44f64-105">Planovi poslovnih Office 365 i Office 365 poslovne Premium uključuju Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="44f64-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="44f64-106">Morate omogućiti [zajedničko računalo aktivacije](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="44f64-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="44f64-107">Ako želite instalirati Office 365 ProPlus na ZAPISI s portala Office 365 ***koji koristi zadane postavke instalacije***, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="44f64-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="44f64-108">Provjerite što Office 365 plan imate.</span><span class="sxs-lookup"><span data-stu-id="44f64-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="44f64-109">Saznajte kako</span><span class="sxs-lookup"><span data-stu-id="44f64-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="44f64-110">Ako je potrebno, prijeđite na drugu Office 365 plan.</span><span class="sxs-lookup"><span data-stu-id="44f64-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="44f64-111">Saznajte kako</span><span class="sxs-lookup"><span data-stu-id="44f64-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="44f64-112">Office već instaliran na poslužitelju ZAPISI pomoću Office 365 planove, deinstalirajte ga.</span><span class="sxs-lookup"><span data-stu-id="44f64-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="44f64-113">Na primjer, odlaskom na upravljačkoj ploči \> deinstalirati program.</span><span class="sxs-lookup"><span data-stu-id="44f64-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="44f64-114">Deinstaliraj pomoću [Microsoft podršku i oporavak pomoćnika](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako se izvodi u problemi.</span><span class="sxs-lookup"><span data-stu-id="44f64-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="44f64-115">Na poslužitelju ZAPISI prijaviti u portala za Office 365 s administratorskog računa i [instalirajte Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="44f64-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="44f64-116">Nakon instalacije Officea ***ne otvorite ili prijaviti*** za sve Officeove aplikacije.</span><span class="sxs-lookup"><span data-stu-id="44f64-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="44f64-117">Na poslužitelju ZAPISI omogućili aktivaciju dijeljenom računalu uređivanjem registra slijedeći ove korake:</span><span class="sxs-lookup"><span data-stu-id="44f64-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="44f64-118">Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite Pokreni.</span><span class="sxs-lookup"><span data-stu-id="44f64-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="44f64-119">U okvir Otvori upišite **regedit**, a zatim odaberite u redu.</span><span class="sxs-lookup"><span data-stu-id="44f64-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="44f64-120">Odaberite da upit o dozvoli uređivač registra da biste napravili promjene na uređaj.</span><span class="sxs-lookup"><span data-stu-id="44f64-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="44f64-121">U uređivač registra, dodajte vrijednost niza **SharedComputerLicensing** s postavkom 1 pod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="44f64-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="44f64-122">Na poslužitelju ZAPISI, ***prijavite se kao krajnji korisnik*** i [Provjerite je li aktivacija dijeljenom računalu omogućen za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="44f64-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="44f64-123">Za dodatne pojedinosti o preduvjeti, upute za postavljanje i prilagođene instalacije pomoću alata za uvođenje Office upute pogledajte [Uvođenje Office 365 ProPlus pomoću udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="44f64-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="44f64-124">Da biste riješili pogreške vezane uz aktivaciju dijeljenom računalu, pogledajte [otklanjanje problema s dijeljenom računalu aktivacije za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="44f64-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  