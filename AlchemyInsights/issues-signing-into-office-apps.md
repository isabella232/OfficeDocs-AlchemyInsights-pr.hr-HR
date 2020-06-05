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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579857"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="01b7a-102">Ispravljanje poruke aplikacije Microsoft 365 "Modul pouzdane platforme vašeg računala ne funkcionira ispravno"</span><span class="sxs-lookup"><span data-stu-id="01b7a-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="01b7a-103">Da biste ispravili tu pogrešku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="01b7a-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="01b7a-104">Instalirajte najnovija ažuriranja za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="01b7a-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="01b7a-105">[Izbrišite vjerodajnice sustava Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="01b7a-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="01b7a-106">**Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0.</span><span class="sxs-lookup"><span data-stu-id="01b7a-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="01b7a-107">(Npr.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="01b7a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="01b7a-108">Isprobajte [postupak oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) da biste ispravili pogreške trusted platform module (TPM).</span><span class="sxs-lookup"><span data-stu-id="01b7a-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="01b7a-109">Postavite EnableADAL = 0 pomoću sljedećih koraka:</span><span class="sxs-lookup"><span data-stu-id="01b7a-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="01b7a-110">Desnom tipkom miša kliknite gumb Start sustava Windows, odaberite **Pokreni**, upišite **regedit**, a zatim odaberite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="01b7a-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="01b7a-111">Odaberite **Da** da biste uređivaču registra omogućili izmjene uređaja.</span><span class="sxs-lookup"><span data-stu-id="01b7a-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="01b7a-112">In Registry Editor, dodati DWORD vrijednost od **EnableADAL** sa postavljanje od **0** pod HKEY_CURRENT_USER\SoftwareMicrosoft\Office16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="01b7a-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="01b7a-113">Dodatne informacije [potražite u odjeljku Problemi s povezivanjem prilikom ažuriranja na međuverziju sustava Office 2016 16.0.7967 u sustavu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="01b7a-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>