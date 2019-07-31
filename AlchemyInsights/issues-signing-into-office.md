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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938158"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="8ca43-102">Potpisivanje Office apps problemi</span><span class="sxs-lookup"><span data-stu-id="8ca43-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="8ca43-103">Da biste riješili probleme za prijavu s Office apps, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="8ca43-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="8ca43-104">Uklonite sve račune rad, osim zahvaćeni račun pomoću Windows postavke > **pristup poslu ili u školi**.</span><span class="sxs-lookup"><span data-stu-id="8ca43-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="8ca43-105">[Očisti Office vjerodajnice](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću Windows upravitelj vjerodajnica.</span><span class="sxs-lookup"><span data-stu-id="8ca43-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="8ca43-106">**Napomena:** Putova registra za Office 2016 ste promijenili 16.0.</span><span class="sxs-lookup"><span data-stu-id="8ca43-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="8ca43-107">(Prije: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="8ca43-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="8ca43-108">Otvorite Office app, odaberite **datoteku** > **račun** > **Odjava**. Zatim prijavite putem korisničkog računa s valjanu licencu.</span><span class="sxs-lookup"><span data-stu-id="8ca43-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="8ca43-109">Za detaljnije informacije pogledajte [račune u Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="8ca43-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="8ca43-110">Za Mac, vidjeti [ne mogu prijaviti u 2016 Office za Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="8ca43-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="8ca43-111">Ako dođe do pogreške pri povezivanju s Office 365 pomoću Office 2013, omogućiti Moderna provjeru autentičnosti klijenta sustava Office.</span><span class="sxs-lookup"><span data-stu-id="8ca43-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="8ca43-112">Dodatne informacije potražite u sljedećem članku:</span><span class="sxs-lookup"><span data-stu-id="8ca43-112">For more information, see:</span></span>
- [<span data-ttu-id="8ca43-113">Ne možete se prijaviti na Office 365, Azure ili Intune</span><span class="sxs-lookup"><span data-stu-id="8ca43-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="8ca43-114">Povezivanjem u prijavu nakon ažuriranja za Office 2016 build 16.0.7967 na Windows 10</span><span class="sxs-lookup"><span data-stu-id="8ca43-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="8ca43-115">"Nažalost, drugi račun iz vaše organizacije već prijavljeni na ovom računalu" u Officeu</span><span class="sxs-lookup"><span data-stu-id="8ca43-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="8ca43-116">Rješavanje problema u znak s Office Moderna provjere autentičnosti kada koristite ADFS</span><span class="sxs-lookup"><span data-stu-id="8ca43-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)