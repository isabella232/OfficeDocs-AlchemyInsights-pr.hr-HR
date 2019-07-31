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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938160"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="e91ce-102">Popravljanje Office apps "Trusted Platform module vaše računalo ne radi ispravno" poruka</span><span class="sxs-lookup"><span data-stu-id="e91ce-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="e91ce-103">Da biste ispravili tu pogrešku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="e91ce-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="e91ce-104">Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="e91ce-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="e91ce-105">[Očisti Office vjerodajnice](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću Windows upravitelj vjerodajnica.</span><span class="sxs-lookup"><span data-stu-id="e91ce-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e91ce-106">**Napomena:** Putova registra za Office 2016 ste promijenili 16.0.</span><span class="sxs-lookup"><span data-stu-id="e91ce-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e91ce-107">(Prije: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e91ce-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="e91ce-108">Pokušajte [postupka oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) da biste ispravili pogreške Trusted Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="e91ce-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="e91ce-109">Postaviti na EnableADAL = 0 pomoću sljedećih koraka:</span><span class="sxs-lookup"><span data-stu-id="e91ce-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="e91ce-110">Desnom tipkom miša pritisnite gumb Start sustava Windows, odaberite **Pokreni**, upišite **regedit**i odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="e91ce-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="e91ce-111">Za odaberite **da** Dopusti uređivač registra da biste napravili promjene na uređaj.</span><span class="sxs-lookup"><span data-stu-id="e91ce-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="e91ce-112">U programu Registry Editor dodajte DWORD vrijednost **EnableADAL** s postavkom **0** pod HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="e91ce-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="e91ce-113">Za dodatne informacije pogledajte [veze problemi u prijavu nakon ažuriranja za Office 2016 build 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="e91ce-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>