---
title: Potpisivanje Office apps problemi
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938159"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="d6b74-102">Prazan prijavu zaslon u Office apps</span><span class="sxs-lookup"><span data-stu-id="d6b74-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="d6b74-103">Da biste riješili taj problem, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="d6b74-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="d6b74-104">Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="d6b74-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="d6b74-105">Vrati mogućnosti programa Internet Explorer: idite na **Alati** > **Internet opcije** > **Napredno** > **Vraćanje postavki programa Internet Explorer** (Napomena će izgubiti prilagođene postavke), a zatim pokušajte ponovno potpisivanja Office.</span><span class="sxs-lookup"><span data-stu-id="d6b74-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="d6b74-106">Onemogući Windows Defender aplikacije Guard (WDAG) ili bilo koji sličan vatrozid ili protuvirusni program:</span><span class="sxs-lookup"><span data-stu-id="d6b74-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="d6b74-107">Na upravljačkoj ploči, idite na **programe**i odabrati **značajke Windows uključivanje ili isključivanje**.</span><span class="sxs-lookup"><span data-stu-id="d6b74-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="d6b74-108">Ako je omogućen Guard aplikacije Windows Defender, pokušajte ga onemogućiti.</span><span class="sxs-lookup"><span data-stu-id="d6b74-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="d6b74-109">**Napomena:** Možda ćete morati ponovo pokrenuti računalo.</span><span class="sxs-lookup"><span data-stu-id="d6b74-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="d6b74-110">Osigurajte da Microsoft.AAD.BrokerPlugin [AAD WAM dodatak](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne blokira aplikacije ili vatrozida/funkcijama za zaštitu-virus program.</span><span class="sxs-lookup"><span data-stu-id="d6b74-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="d6b74-111">[Očisti Office vjerodajnice](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću Windows upravitelj vjerodajnica.</span><span class="sxs-lookup"><span data-stu-id="d6b74-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d6b74-112">**Napomena:** Putova registra za Office 2016 ste promijenili 16.0.</span><span class="sxs-lookup"><span data-stu-id="d6b74-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d6b74-113">(Prije: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d6b74-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="d6b74-114">Za dodatne informacije pogledajte [veze problemi u prijavu nakon ažuriranja za Office 2016 build 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="d6b74-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>