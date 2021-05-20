---
title: 2681 Attack Simulator u Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545718"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="95293-102">Napad u Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="95293-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="95293-103">Nedostaje li vam simulator napada?</span><span class="sxs-lookup"><span data-stu-id="95293-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="95293-104">U programu Attack Simulator **potreban je Microsoft Defender Office 365 plan 2** ili Office 365 Enterprise **E5**.</span><span class="sxs-lookup"><span data-stu-id="95293-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="95293-105">Simulator napada nije **obuhvaćen** programom Microsoft Defender za Office 365 plan 1, Office 365 Enterprise E3 ili bilo koju Microsoft 365 Apps za male tvrtke pretplatu.</span><span class="sxs-lookup"><span data-stu-id="95293-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="95293-106">Račun koji koristite za pokretanje simuliranih napada zahtijeva dozvole globalnog administratora ili administratora sigurnosti i višestruku provjeru autentičnosti (MFA).</span><span class="sxs-lookup"><span data-stu-id="95293-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="95293-107">Dodatne informacije o preduvjetima za Napad na simulatoru potražite [u ovoj temi](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="95293-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="95293-108">Važne stvari koje je važno znati o **simulacijama** napada lozinkom na silu:</span><span class="sxs-lookup"><span data-stu-id="95293-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="95293-109">Ako je ciljni račun omogućio MFA, a lozinka je pravilno odabrana, račun se neće prikazati kao ugrožen (drugi faktor provjere autentičnosti bit će nepotpun).</span><span class="sxs-lookup"><span data-stu-id="95293-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="95293-110">Datoteka lozinke ne smije biti veća od 10 MB.</span><span class="sxs-lookup"><span data-stu-id="95293-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="95293-111">Upotrijebite jednu lozinku po retku i nakon zadnje lozinke na popisu uvrsti praznu crtu (povrat prijevoza).</span><span class="sxs-lookup"><span data-stu-id="95293-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="95293-112">Važne stvari koje je važno znati o krađi **identiteta koplja prilaganje** simulacija:</span><span class="sxs-lookup"><span data-stu-id="95293-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="95293-113">Prema dizajnu ne možete navesti prilagođenu vrijednost ZA URL poslužitelja za prijavu **u krađu identiteta.**</span><span class="sxs-lookup"><span data-stu-id="95293-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="95293-114">Ako primatelj koristi dodatak Omogući poruku izvješća da bi prijavio poruku kao krađu identiteta, možda ne primate upozorenja za poruku (jer je [to](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) simulirani napad).</span><span class="sxs-lookup"><span data-stu-id="95293-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="95293-115">Izvješća: kada simulirani napad završi, možete kliknuti Detalji o **napadu da** biste vidjeli izvješće.</span><span class="sxs-lookup"><span data-stu-id="95293-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="95293-116">Detaljne upute i nove značajke u programu Attack Simulator potražite u članku [Napad u Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="95293-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
