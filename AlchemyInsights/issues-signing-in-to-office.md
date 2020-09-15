---
title: Problemi s prijavom u aplikacije Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695279"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="6fdd6-102">Prazni zaslon za prijavu u aplikacijama Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6fdd6-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="6fdd6-103">Da biste riješili taj problem, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="6fdd6-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="6fdd6-104">Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="6fdd6-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="6fdd6-105">Ponovno postavljanje mogućnosti u pregledniku Internet Explorer: Idite na **Alati**za  >  **napredne internetske mogućnosti**  >  **Advanced**  >  **ponovno postavljanje postavki preglednika Internet Explorer** (primijetite da ćete izgubiti prilagođene postavke), a zatim se pokušajte ponovno prijaviti u Office.</span><span class="sxs-lookup"><span data-stu-id="6fdd6-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="6fdd6-106">Onemogućite čuvar aplikacije programa Windows Defender (WDAG) ili bilo koji sličan vatrozid ili protuvirusni program:</span><span class="sxs-lookup"><span data-stu-id="6fdd6-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="6fdd6-107">Na upravljačkoj ploči otvorite **program**, a zatim odaberite **Uključivanje i isključivanje značajki sustava Windows**.</span><span class="sxs-lookup"><span data-stu-id="6fdd6-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="6fdd6-108">Ako je omogućen čuvar aplikacije programa Windows Defender, pokušajte ga onemogućiti.</span><span class="sxs-lookup"><span data-stu-id="6fdd6-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="6fdd6-109">**Upozorenje:** Možda ćete morati ponovno pokrenuti računalo.</span><span class="sxs-lookup"><span data-stu-id="6fdd6-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="6fdd6-110">Provjerite nije li dodatak Microsoft. AAD. [brokerskog dodatka AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nije blokiran bilo kojim aplikacijom ili vatrozidom/antivirusni programom.</span><span class="sxs-lookup"><span data-stu-id="6fdd6-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="6fdd6-111">[Poništite vjerodajnice sustava Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica za Windows.</span><span class="sxs-lookup"><span data-stu-id="6fdd6-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6fdd6-112">**Upozorenje:** Putevi registra za Office 2016 promijenili su se u 16,0.</span><span class="sxs-lookup"><span data-stu-id="6fdd6-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6fdd6-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="6fdd6-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="6fdd6-114">Dodatne informacije potražite u članku [Problemi s povezivanjem u programu za prijavu nakon ažuriranja na Office 2016 međuverzija 16.0.7967 u sustavu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="6fdd6-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>