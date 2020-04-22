---
title: Instalacija sustava na terminalski poslužitelj – bez licence
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
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763209"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="be676-102">Instalacija sustava Office na terminalski poslužitelj</span><span class="sxs-lookup"><span data-stu-id="be676-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="be676-103">Za implementaciju aplikacija microsoft 365 za tvrtke na Windows Server pomoću servisa Udaljene radne površine (RDS), ranije nazvane Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="be676-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="be676-104">Morate imati pretplatu na Microsoft 365 koja obuhvaća Aplikacije sustava Microsoft 365 za tvrtke, kao što su Office 365 Enterprise E3 ili Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="be676-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="be676-105">Tarife Microsoft 365 Apps for business i Microsoft 365 Apps for business Premium ne obuhvaćaju Aplikacije za Microsoft 365 za tvrtke.</span><span class="sxs-lookup"><span data-stu-id="be676-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="be676-106">Morate omogućiti [aktivaciju dijeljenog računala](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="be676-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="be676-107">Ako želite instalirati Microsoft 365 aplikacije za tvrtke na RDS iz centra za administratore sustava Microsoft 365, ***koji koristi zadane postavke instalacije,*** slijedite ove korake.</span><span class="sxs-lookup"><span data-stu-id="be676-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="be676-108">Microsoftov [pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) možete preuzeti i pokrenuti da biste instalirali Microsoft 365 Aplikacije za tvrtke u načinu aktivacije dijeljenog računala.</span><span class="sxs-lookup"><span data-stu-id="be676-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="be676-109">Provjerite koju pretplatu na Microsoft 365 imate.</span><span class="sxs-lookup"><span data-stu-id="be676-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="be676-110">Saznajte kako</span><span class="sxs-lookup"><span data-stu-id="be676-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="be676-111">Ako je potrebno, prijeđite na drugu pretplatu na Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="be676-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="be676-112">Saznajte kako</span><span class="sxs-lookup"><span data-stu-id="be676-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="be676-113">Ako je Office već instaliran na RDS poslužitelju pomoću bilo koje druge pretplate na Microsoft 365, deinstalirajte ga.</span><span class="sxs-lookup"><span data-stu-id="be676-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="be676-114">Na primjer, tako da \> odete na Upravljačku ploču Deinstalirajte program.</span><span class="sxs-lookup"><span data-stu-id="be676-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="be676-115">Ako imate problema, deinstalirajte pomoću [Microsoftova pomoćnika za podršku i oporavak.](https://aka.ms/SARA-OfficeUninstall-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="be676-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="be676-116">Na RDS poslužitelju prijavite se u centar za administratore sustava Microsoft 365 pomoću administratorskog računa i [instalirajte Microsoft 365 Apps za tvrtke](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="be676-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="be676-117">Nakon instalacije sustava Office ***nemojte otvarati aplikacije*** sustava Office niti se prijaviti u ih.</span><span class="sxs-lookup"><span data-stu-id="be676-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="be676-118">Na RDS poslužitelju omogućite aktivaciju zajedničkog računala uređivanjem registra slijedeći ove korake:</span><span class="sxs-lookup"><span data-stu-id="be676-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="be676-119">Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite Pokreni.</span><span class="sxs-lookup"><span data-stu-id="be676-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="be676-120">U okvir Otvori upišite **regedit**, a zatim odaberite U redu.</span><span class="sxs-lookup"><span data-stu-id="be676-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="be676-121">Odaberite Da kada se od vas zatraži da dopustite uređivaču registra da unese promjene na uređaj.</span><span class="sxs-lookup"><span data-stu-id="be676-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="be676-122">In Registry Editor, dodati vrpca vrijednost od **SharedComputerLicensing** sa postavljanje od 1 pod HKEY_LOCAL_MACHINESOFTWAREMicrosoftOfficeClickToRunConfiguration\\\\.</span><span class="sxs-lookup"><span data-stu-id="be676-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="be676-123">Na RDS poslužitelju ***prijavite se kao krajnji korisnik*** i provjerite je li [aktivacija zajedničkog računala omogućena za Microsoft 365 Aplikacije za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="be676-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="be676-124">Dodatne informacije o preduvjetima, uputama za postavljanje i smjernicama o prilagođenim instalacijama pomoću alata za implementaciju sustava Office [potražite u članku Implementacija aplikacija microsoft 365 za tvrtke pomoću servisa Udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="be676-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="be676-125">Da biste ispravili pogreške vezane uz aktivaciju zajedničkog računala, [pročitajte članak Otklanjanje poteškoća s aktivacijom zajedničkog računala za Aplikacije sustava Microsoft 365 za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="be676-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  