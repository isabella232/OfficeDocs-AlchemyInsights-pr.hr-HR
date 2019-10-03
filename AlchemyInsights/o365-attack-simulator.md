---
title: 2681 napad simulator u Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305324"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="abd71-102">Napad simulator u Office 365</span><span class="sxs-lookup"><span data-stu-id="abd71-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="abd71-103">Da li ti nedostaje simulator napada?</span><span class="sxs-lookup"><span data-stu-id="abd71-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="abd71-104">Napad simulator zahtijeva **Office 365 napredni plan zaštite prijetnji 2 (ATP plan 2)** ili **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="abd71-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="abd71-105">Simulator napada nije **uključen u** Office 365 napredni plan zaštite prijetnji 1 (ATP plan 1), Office 365 Enterprise E3 ili bilo koje Office 365 poslovne pretplate.</span><span class="sxs-lookup"><span data-stu-id="abd71-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="abd71-106">Račun koji koristite za pokretanje simulirane napade zahtijeva globalne administratorske ili sigurnosne administratorske dozvole i multi-faktor autentikacije (MFP).</span><span class="sxs-lookup"><span data-stu-id="abd71-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="abd71-107">Dodatne informacije o zahtjevima simulator napada pogledajte [ovu temu](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="abd71-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="abd71-108">Važne stvari koje morate znati o **brutalnoj sile lozinke** napada simulacije:</span><span class="sxs-lookup"><span data-stu-id="abd71-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="abd71-109">Ako ciljni račun ima MFA omogućen i lozinka je pogodio ispravno, račun neće prikazati kao ugrožen (drugi faktor provjere autentičnosti će biti nepotpun).</span><span class="sxs-lookup"><span data-stu-id="abd71-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="abd71-110">Datoteka lozinke ne može biti veća od 10 MB.</span><span class="sxs-lookup"><span data-stu-id="abd71-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="abd71-111">Upotrijebite jednu lozinku po retku i uključite praznu liniju (povratni prijevoz) nakon posljednje lozinke na popisu.</span><span class="sxs-lookup"><span data-stu-id="abd71-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="abd71-112">Važne stvari za znati o **koplja phishing** priložiti simulacije:</span><span class="sxs-lookup"><span data-stu-id="abd71-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="abd71-113">Po dizajnu, ne možete pružiti prilagođenu vrijednost za **URL poslužitelja za prijavu krađe identiteta**.</span><span class="sxs-lookup"><span data-stu-id="abd71-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="abd71-114">Ako primatelj koristi [Omogući dodatak poruka izvještaja](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) da bi prijavio poruku kao krađu identiteta, možda nećete primiti upozorenja za poruku (jer je to simulirani napad).</span><span class="sxs-lookup"><span data-stu-id="abd71-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="abd71-115">Izvješća: nakon što je simulirani napad dovršen, možete kliknuti **napad detalji** da biste vidjeli izvješće.</span><span class="sxs-lookup"><span data-stu-id="abd71-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="abd71-116">Za detaljne upute i nove značajke u napad simulator, pogledajte [napad simulator u Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="abd71-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>