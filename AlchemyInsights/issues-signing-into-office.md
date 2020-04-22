---
title: Problemi s prijavom u aplikacije sustava Office
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762971"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="70a47-102">Problemi s prijavom u aplikacije sustava Office</span><span class="sxs-lookup"><span data-stu-id="70a47-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="70a47-103">Da biste riješili probleme s prijavom u aplikacije sustava Office, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="70a47-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="70a47-104">Uklonite sve poslovne račune, osim zahvaćenog računa, pomoću postavki sustava Windows > **Access work ili school**.</span><span class="sxs-lookup"><span data-stu-id="70a47-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="70a47-105">[Izbrišite vjerodajnice sustava Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="70a47-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="70a47-106">**Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0.</span><span class="sxs-lookup"><span data-stu-id="70a47-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="70a47-107">(npr.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="70a47-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="70a47-108">Otvorite aplikaciju sustava Office, odaberite > **Odjava\*\*\*\*računa datoteke** **File** > . Zatim se prijavite pomoću korisničkog računa s valjanom licencom.</span><span class="sxs-lookup"><span data-stu-id="70a47-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="70a47-109">Detaljne informacije potražite u članku [Računi u sustavu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="70a47-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="70a47-110">Za Mac pročitajte [Nije moguća prijava u aplikaciju sustava Office 2016 za Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="70a47-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="70a47-111">Ako se pojave pogreške tijekom povezivanja sa sustavom Microsoft 365 pomoću sustava Office 2013, omogućite modernu provjeru autentičnosti za klijent sustava Office.</span><span class="sxs-lookup"><span data-stu-id="70a47-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="70a47-112">Dodatne informacije potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="70a47-112">For more information, see:</span></span>
- [<span data-ttu-id="70a47-113">Ne možete se prijaviti u Microsoft 365, Azure ili Intune</span><span class="sxs-lookup"><span data-stu-id="70a47-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="70a47-114">Problemi s povezivanjem prilikom prijave nakon ažuriranja za Office 2016 build 16.0.7967 u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="70a47-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="70a47-115">"Nažalost, drugi račun vaše tvrtke ili ustanove već je prijavljen na ovom računalu" u sustavu Office</span><span class="sxs-lookup"><span data-stu-id="70a47-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="70a47-116">Otklanjanje poteškoća s prijavom pomoću moderne provjere autentičnosti sustava Office kada koristite ADFS</span><span class="sxs-lookup"><span data-stu-id="70a47-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)