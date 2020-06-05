---
title: Problemi s prijavom u aplikacije sustava Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579893"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="6b540-102">Prazan zaslon za prijavu u aplikacijama Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6b540-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="6b540-103">Da biste riješili taj problem, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="6b540-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="6b540-104">Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="6b540-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="6b540-105">Vraćanje izvornih mogućnosti preglednika Internet Explorer: idite na **Alati**  >  **Internetske mogućnosti**  >  **Advanced**  >  **Napredne postavke preglednika Internet Explorer** (imajte na umu da ćete izgubiti prilagođene postavke), a zatim se ponovno pokušajte prijaviti u Office.</span><span class="sxs-lookup"><span data-stu-id="6b540-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="6b540-106">Onesposobiti Windows Branitelj Aplikacija Čuvati (WDAG) ili bilo koji sličan firewall ili protu-- virus plan:</span><span class="sxs-lookup"><span data-stu-id="6b540-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="6b540-107">Na upravljačkoj ploči idite na **Programi**, a zatim uključite **ili isključite značajke sustava Windows**.</span><span class="sxs-lookup"><span data-stu-id="6b540-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="6b540-108">Ako je windows defender application guard omogućen, pokušajte ga onemogućiti.</span><span class="sxs-lookup"><span data-stu-id="6b540-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="6b540-109">**Napomena:** Možda ćete morati ponovo pokrenuti računalo.</span><span class="sxs-lookup"><span data-stu-id="6b540-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="6b540-110">Provjerite da dodatak Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne blokira nijedan program za aplikaciju ili vatrozid/protuvirusni program.</span><span class="sxs-lookup"><span data-stu-id="6b540-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="6b540-111">[Izbrišite vjerodajnice sustava Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="6b540-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6b540-112">**Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0.</span><span class="sxs-lookup"><span data-stu-id="6b540-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6b540-113">(Npr.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="6b540-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="6b540-114">Dodatne informacije [potražite u odjeljku Problemi s povezivanjem prilikom ažuriranja na međuverziju sustava Office 2016 16.0.7967 u sustavu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="6b540-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>