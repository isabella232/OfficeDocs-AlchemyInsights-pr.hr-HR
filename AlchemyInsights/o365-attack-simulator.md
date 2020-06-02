---
title: 2681 simulator napada u sustavu Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506730"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="84696-102">Simulator napada u sustavu Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="84696-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="84696-103">Nedostaje li vam simulator napada?</span><span class="sxs-lookup"><span data-stu-id="84696-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="84696-104">Za simulator napada potreban je **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** ili **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="84696-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="84696-105">Simulator napada **nije** obuhvaćen office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 ili bilo koje Aplikacije microsoft 365 za tvrtke pretplate.</span><span class="sxs-lookup"><span data-stu-id="84696-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="84696-106">Račun koji koristite za pokretanje simuliranih napada zahtijeva globalne administratorske dozvole ili administratorske dozvole za sigurnost i višestruku provjeru autentičnosti (MFA).</span><span class="sxs-lookup"><span data-stu-id="84696-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="84696-107">Dodatne informacije o zahtjevima attack simulatora potražite [u ovoj temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="84696-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="84696-108">Važne stvari koje treba znati o **Brute Force Lozinka** napad simulacije:</span><span class="sxs-lookup"><span data-stu-id="84696-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="84696-109">Ako ciljni račun ima omogućen MFA i lozinka je ispravno pogodila, račun se neće prikazati kao ugrožen (drugi faktor provjere autentičnosti će biti nepotpun).</span><span class="sxs-lookup"><span data-stu-id="84696-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="84696-110">Datoteka lozinke ne može biti veća od 10 MB.</span><span class="sxs-lookup"><span data-stu-id="84696-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="84696-111">Upotrijebite jednu lozinku po retku i uključite prazan redak (prijevoz povratak) nakon zadnje lozinke na popisu.</span><span class="sxs-lookup"><span data-stu-id="84696-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="84696-112">Važne stvari koje treba znati o **Spear Phishing** priložiti simulacije:</span><span class="sxs-lookup"><span data-stu-id="84696-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="84696-113">Po dizajnu ne možete navesti prilagođenu vrijednost za URL poslužitelja za **prijavu za phishing**.</span><span class="sxs-lookup"><span data-stu-id="84696-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="84696-114">Ako primatelj koristi [dodatak Omogući poruku izvješća](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) da bi prijavio poruku kao krađu identiteta, možda nećete primiti upozorenja za poruku (jer je to simulirani napad).</span><span class="sxs-lookup"><span data-stu-id="84696-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="84696-115">Izvješća: nakon dovršetka simuliranog napada možete kliknuti **Detalji napada** da biste vidjeli izvješće.</span><span class="sxs-lookup"><span data-stu-id="84696-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="84696-116">Detaljne upute i nove značajke u aplikaciji Attack Simulator potražite u [odjeljku Simulator napada u sustavu Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="84696-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
