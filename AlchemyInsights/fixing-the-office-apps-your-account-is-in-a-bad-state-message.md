---
title: Popravljanje aplikacija sustava Office Vaš račun nalazi se u poruci o lošem stanju
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969297"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="dfa72-102">Ispravljanje pogreške u vezi s aplikacijama sustava Office "Vaš račun je u lošem stanju"</span><span class="sxs-lookup"><span data-stu-id="dfa72-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="dfa72-103">Da biste riješili tu pogrešku, isprobajte sljedeće mogućnosti na zahvaćenom računalu:</span><span class="sxs-lookup"><span data-stu-id="dfa72-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="dfa72-104">Otvorite aplikaciju sustava Office, odaberite Odjava**na račun** >  **datoteke** > **sa svih računa**.</span><span class="sxs-lookup"><span data-stu-id="dfa72-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="dfa72-105">Ponovno se prijavite pomoću korisničkog računa s valjanom licencom.</span><span class="sxs-lookup"><span data-stu-id="dfa72-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="dfa72-106">Detaljne informacije potražite [u odjeljku Računi u sustavu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="dfa72-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="dfa72-107">[Izbrišite vjerodajnice sustava Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="dfa72-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="dfa72-108">**Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0.</span><span class="sxs-lookup"><span data-stu-id="dfa72-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="dfa72-109">Na primjer, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="dfa72-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="dfa72-110">Na zahvaćenom računalu postavite EnableADAL = 0 pomoću sljedećih koraka:</span><span class="sxs-lookup"><span data-stu-id="dfa72-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="dfa72-111">Desnom tipkom miša kliknite gumb Windows i odaberite **Pokreni**.</span><span class="sxs-lookup"><span data-stu-id="dfa72-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="dfa72-112">U okvir **Otvori** upišite **regedit**, a zatim odaberite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="dfa72-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="dfa72-113">Odaberite **Da** kada se od vas zatraži da biste uređivaču registra dopustili izmjene uređaja.</span><span class="sxs-lookup"><span data-stu-id="dfa72-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="dfa72-114">U uređivaču registra dodajte DWORD vrijednost EnableADAL s postavkom 0 pod HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="dfa72-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="dfa72-115">Ako dođe do pogreške tijekom povezivanja sa sustavom Office 365 pomoću sustava Office 2013, [omogućite modernu provjeru autentičnosti](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) klijenta sustava Office.</span><span class="sxs-lookup"><span data-stu-id="dfa72-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="dfa72-116">Dodatne informacije potražite u [odjeljku Otklanjanje poteškoća s aplikacijama koje se ne mogu prijaviti u Office 365, Azure ili Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="dfa72-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

