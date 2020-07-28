---
title: Upravljanje automatskim ažuriranjima za aplikacije sustava Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438838"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="fa87b-102">Upravljanje automatskim ažuriranjima za aplikacije sustava Office</span><span class="sxs-lookup"><span data-stu-id="fa87b-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="fa87b-103">Ažuriranja za aplikacije sustava Office prema zadanim se postavkama automatski preuzimaju i primjenjuju u pozadini bez intervencije korisnika.</span><span class="sxs-lookup"><span data-stu-id="fa87b-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="fa87b-104">Međutim, administratori mogu kontrolirati kako se ažuriranja primjenjuju pomoću postavki servisa Office Update.</span><span class="sxs-lookup"><span data-stu-id="fa87b-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="fa87b-105">Postavke ažuriranja administratorima omogućuju omogućivanje ili onemogućivanje automatskog ažuriranja, prikaz ili skrivanje gumba **Ažuriraj sada** u sustavu Office, postavite rokove ažuriranja i još mnogo toga.</span><span class="sxs-lookup"><span data-stu-id="fa87b-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="fa87b-106">Detaljne informacije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="fa87b-106">For detailed information, see:</span></span>

- [<span data-ttu-id="fa87b-107">Konfiguriranje postavki ažuriranja za Office</span><span class="sxs-lookup"><span data-stu-id="fa87b-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="fa87b-108">Automatsko ažuriranje za Office nije omogućeno</span><span class="sxs-lookup"><span data-stu-id="fa87b-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="fa87b-109">Definiranje načina ažuriranja sustava Office nakon instalacije</span><span class="sxs-lookup"><span data-stu-id="fa87b-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="fa87b-110">Da biste pregledali postojeće postavke ažuriranja primijenjene na klijentsko računalo, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="fa87b-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="fa87b-111">OpenBSD Registry Editor odlaskom na **Početak**  >  **Trčanje**  >  **regentstvo.**</span><span class="sxs-lookup"><span data-stu-id="fa87b-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="fa87b-112">Prijeđite na sljedeće mjesto i pregledajte postavke ažuriranja sustava Office:</span><span class="sxs-lookup"><span data-stu-id="fa87b-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="fa87b-113">A.</span><span class="sxs-lookup"><span data-stu-id="fa87b-113">a.</span></span> <span data-ttu-id="fa87b-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="fa87b-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="fa87b-115">B.</span><span class="sxs-lookup"><span data-stu-id="fa87b-115">b.</span></span> <span data-ttu-id="fa87b-116">ClickToRun\Konfiguracija</span><span class="sxs-lookup"><span data-stu-id="fa87b-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="fa87b-117">**Napomena:**  Ako je postavljen ključ OfficeMgmtCOM, **možda**će vam se prikazati poruka "Ažuriranjima upravlja administrator sustava" u  >  **Account**  >  **ažuriranjima sustava Office**Account Office .</span><span class="sxs-lookup"><span data-stu-id="fa87b-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="fa87b-118">Dodatne informacije [potražite u odjeljku Upravljanje ažuriranjima aplikacija microsoft 365 s programom Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="fa87b-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  