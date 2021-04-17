---
title: Problemi prilikom prijave u aplikacije sustava Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833023"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="57584-102">Prazan zaslon za prijavu u aplikacije Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="57584-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="57584-103">Da biste riješili taj problem, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="57584-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="57584-104">Instalirajte najnovija ažuriranja za [Windows i](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="57584-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="57584-105">Ponovno postavite mogućnosti preglednika Internet Explorer: otvorite Alati za internetske mogućnosti Napredno ponovno postavljanje postavki preglednika Internet Explorer (imajte na umu da ćete izgubiti prilagođene postavke), a  >    >    >   zatim se ponovno pokušajte prijaviti u Office.</span><span class="sxs-lookup"><span data-stu-id="57584-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="57584-106">Onemogućite Windows Defender Application Guard (WDAG) ili bilo koji sličan vatrozid ili antivirusni program:</span><span class="sxs-lookup"><span data-stu-id="57584-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="57584-107">Na upravljačkoj ploči idite **na Programi**, a zatim **odaberite Uključi ili isključi značajke sustava Windows**.</span><span class="sxs-lookup"><span data-stu-id="57584-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="57584-108">Ako je omogućen Windows Defender Application Guard, pokušajte ga onemogućiti.</span><span class="sxs-lookup"><span data-stu-id="57584-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="57584-109">**Napomena:** Možda ćete morati ponovno pokrenuti računalo.</span><span class="sxs-lookup"><span data-stu-id="57584-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="57584-110">Provjerite ne blokira li programski dodatak Microsoft.AAD.BrokerPlugin [AAD WAM.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)</span><span class="sxs-lookup"><span data-stu-id="57584-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="57584-111">[Poništite vjerodajnice sustava Office pomoću](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) upravitelja vjerodajnica sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="57584-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="57584-112">**Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0.</span><span class="sxs-lookup"><span data-stu-id="57584-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="57584-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="57584-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="57584-114">Dodatne informacije potražite u članku Problemi s povezivanjem prilikom prijave nakon ažuriranja na međuverziju [16.0.7967 sustava Office 2016 u sustavu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="57584-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>