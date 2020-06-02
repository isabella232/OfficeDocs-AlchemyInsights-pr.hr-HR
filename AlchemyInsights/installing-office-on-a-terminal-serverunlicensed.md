---
title: Instaliranje ureda na terminalskom poslužitelju - Nelicencirana
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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508620"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="9f741-102">Instaliranje sustava Office na terminalski poslužitelj</span><span class="sxs-lookup"><span data-stu-id="9f741-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="9f741-103">Za implementaciju aplikacija sustava Microsoft 365 za tvrtke na Windows Serveru pomoću servisa udaljene radne površine (RDS), koji su prethodno imenovani servisima Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="9f741-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="9f741-104">Morate imati pretplatu na Microsoft 365 koja obuhvaća Aplikacije microsoft 365 za tvrtke, kao što su Office 365 Enterprise E3 ili Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="9f741-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="9f741-105">Tarife za Microsoft 365 aplikacije za tvrtke i Microsoft 365 Aplikacije za tvrtke Premium ne obuhvaćaju Microsoft 365 Aplikacije za tvrtke.</span><span class="sxs-lookup"><span data-stu-id="9f741-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="9f741-106">Morate omogućiti [aktivaciju dijeljenog računala](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="9f741-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="9f741-107">Ako želite instalirati Microsoft 365 Apps za poduzeće na RDS iz centra za administratore sustava Microsoft 365, ***koji koristi zadane postavke instalacije, slijedite***ove korake.</span><span class="sxs-lookup"><span data-stu-id="9f741-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="9f741-108">[Microsoftov pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) možete preuzeti i pokrenuti da biste instalirali Microsoft 365 Apps za tvrtke u načinu aktivacije dijeljenog računala.</span><span class="sxs-lookup"><span data-stu-id="9f741-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="9f741-109">Provjerite imate li pretplatu na Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9f741-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="9f741-110">Saznajte kako</span><span class="sxs-lookup"><span data-stu-id="9f741-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="9f741-111">Ako je potrebno, prijeđite na drugu pretplatu na Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9f741-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="9f741-112">Saznajte kako</span><span class="sxs-lookup"><span data-stu-id="9f741-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="9f741-113">Ako je Office već instaliran na RDS poslužitelju pomoću bilo koje druge pretplate na Microsoft 365, deinstalirajte je.</span><span class="sxs-lookup"><span data-stu-id="9f741-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="9f741-114">Na primjer, tako da odete na \> Deinstalaciju programa na upravljačkoj ploči.</span><span class="sxs-lookup"><span data-stu-id="9f741-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="9f741-115">Deinstalirajte pomoću [Microsoftova pomoćnika za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako naišate na probleme.</span><span class="sxs-lookup"><span data-stu-id="9f741-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="9f741-116">Na RDS poslužitelju prijavite se u centar za administratore sustava Microsoft 365 pomoću administratorskog računa i [instalirajte Microsoft 365 Apps za tvrtke](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="9f741-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="9f741-117">Nakon instalacije sustava Office ***nemojte otvarati niti se prijavjeti u*** bilo koje aplikacije sustava Office.</span><span class="sxs-lookup"><span data-stu-id="9f741-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="9f741-118">Na RDS poslužitelju omogućite aktivaciju zajedničkog računala uređivanjem registra slijedeći ove korake:</span><span class="sxs-lookup"><span data-stu-id="9f741-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="9f741-119">Desnom tipkom miša kliknite gumb Windows u donjem lijevom kutu zaslona i odaberite Pokreni.</span><span class="sxs-lookup"><span data-stu-id="9f741-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="9f741-120">U okvir Otvori upišite **regedit**, a zatim odaberite U redu.</span><span class="sxs-lookup"><span data-stu-id="9f741-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="9f741-121">Odaberite Da kada se to od vas zatraži da dopustite uređivaču registra da unesete promjene na uređaju.</span><span class="sxs-lookup"><span data-stu-id="9f741-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="9f741-122">U uređivaču registra dodajte vrijednost niza **SharedComputerLicensing** s postavkom 1 pod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="9f741-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="9f741-123">Na RDS poslužitelju ***prijavite se kao krajnji korisnik*** i provjerite je li [aktivacija dijeljenog računala omogućena za Microsoft 365 Apps za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="9f741-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="9f741-124">Dodatne informacije o preduvjetima, uputama za postavljanje i smjernicama o prilagođenim instalacijama pomoću alata za implementaciju sustava Office potražite [u članku Implementacija aplikacija microsoft 365 za tvrtke pomoću servisa udaljene radne površine](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="9f741-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="9f741-125">Da biste ispravili pogreške povezane s aktivacijom dijeljenog računala, [pročitajte članak Otklanjanje poteškoća s aktivacijom dijeljenog računala za Aplikacije Microsoft 365 za tvrtke](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="9f741-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  