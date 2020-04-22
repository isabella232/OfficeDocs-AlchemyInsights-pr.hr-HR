---
title: 2681 Napadač simulator u Microsoft 365
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
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713458"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="3ea7f-102">Simulator napada u sustavu Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3ea7f-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="3ea7f-103">Nedostaje li ti simulator napada?</span><span class="sxs-lookup"><span data-stu-id="3ea7f-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="3ea7f-104">Attack Simulator zahtijeva **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** ili **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="3ea7f-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="3ea7f-105">Attack Simulator **nije** obuhvaćen Tarifom za zaštitu od 1 (ATP plan 1), Office 365 Enterprise E3 ili pretplatom na Microsoft 365 za tvrtke.</span><span class="sxs-lookup"><span data-stu-id="3ea7f-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="3ea7f-106">Račun koji koristite za pokretanje simuliranih napada zahtijeva dozvole globalnog administratora ili administratora sigurnosti i višestruku provjeru autentičnosti (MFA).</span><span class="sxs-lookup"><span data-stu-id="3ea7f-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="3ea7f-107">Dodatne informacije o preduvjetima attack simulatora potražite [u ovoj temi](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="3ea7f-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="3ea7f-108">Važne stvari koje treba znati o **Brute Force Password** napad simulacije:</span><span class="sxs-lookup"><span data-stu-id="3ea7f-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="3ea7f-109">Ako je ciljnom računu omogućen MFA i lozinka je ispravno postavljena, račun se neće prikazati kao kompromitiran (drugi faktor provjere autentičnosti bit će nepotpun).</span><span class="sxs-lookup"><span data-stu-id="3ea7f-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="3ea7f-110">Datoteka lozinke ne može biti veća od 10 MB.</span><span class="sxs-lookup"><span data-stu-id="3ea7f-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="3ea7f-111">Upotrijebite jednu lozinku po retku i uključite prazan redak (povratak vagona) nakon zadnje lozinke na popisu.</span><span class="sxs-lookup"><span data-stu-id="3ea7f-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="3ea7f-112">Važne stvari koje treba znati o **Spear Phishing** priložiti simulacije:</span><span class="sxs-lookup"><span data-stu-id="3ea7f-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="3ea7f-113">Prema dizajnu, ne možete pružiti prilagođenu vrijednost za **URL poslužitelja za prijavu od krađe identiteta**.</span><span class="sxs-lookup"><span data-stu-id="3ea7f-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="3ea7f-114">Ako primatelj koristi [dodatak Omogući poruku izvješća](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) da bi prijavio poruku kao krađu identiteta, možda nećete primiti upozorenja za poruku (jer je to simulirani napad).</span><span class="sxs-lookup"><span data-stu-id="3ea7f-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="3ea7f-115">Izvješća: nakon dovršetka simuliranog napada možete kliknuti **Detalji o napadu** da biste vidjeli izvješće.</span><span class="sxs-lookup"><span data-stu-id="3ea7f-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="3ea7f-116">Detaljne upute i nove značajke u attack simulatoru potražite [u odjeljku Attack Simulator u sustavu Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="3ea7f-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
