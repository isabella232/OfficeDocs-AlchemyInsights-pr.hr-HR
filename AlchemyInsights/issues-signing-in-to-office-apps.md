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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579929"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="84c4a-102">Ispravak poruke aplikacije sustava Microsoft 365 "Nažalost, već je prijavljen drugi račun iz tvrtke ili ustanove"</span><span class="sxs-lookup"><span data-stu-id="84c4a-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="84c4a-103">Da biste ispravili tu pogrešku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="84c4a-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="84c4a-104">Uklonite sve poslovne račune, osim zahvaćenog računa, pomoću postavki sustava Windows > **Access posao ili školu**.</span><span class="sxs-lookup"><span data-stu-id="84c4a-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="84c4a-105">[Izbrišite vjerodajnice sustava Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="84c4a-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="84c4a-106">**Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0.</span><span class="sxs-lookup"><span data-stu-id="84c4a-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="84c4a-107">(Npr.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="84c4a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="84c4a-108">Otvorite aplikaciju **File**sustava Office, odaberite  >  Odjava**računa**  >  **datoteke**. Zatim se prijavite pomoću korisničkog računa s valjanom licencom.</span><span class="sxs-lookup"><span data-stu-id="84c4a-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="84c4a-109">Detaljne informacije potražite u članku [Računi u sustavu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="84c4a-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="84c4a-110">Za Mac pročitajte [Nije moguća prijava u aplikaciju sustava Office 2016 za Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="84c4a-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="84c4a-111">Dodatne informacije potražite [u odjeljku "Nažalost, na ovom je računalu već prijavljen drugi račun tvrtke ili ustanove" u sustavu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="84c4a-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>