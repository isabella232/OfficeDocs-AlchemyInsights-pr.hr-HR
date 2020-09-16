---
title: 2681 simulator napada u programu Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759211"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="b9cc4-102">Simulator napada u programu Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b9cc4-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="b9cc4-103">Jeste li propustili Attack simulator?</span><span class="sxs-lookup"><span data-stu-id="b9cc4-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="b9cc4-104">Simulator napada zahtijeva **office 365 napredni plan zaštite prijetnje 2 (ATP plan 2)** ili **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="b9cc4-105">Simulator napada nije **uključen u** Office 365 napredni plan zaštite prijetnje 1 (ATP tarifa 1), Office 365 Enterprise E3 ili bilo koje Microsoftove pretplate za tvrtke Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="b9cc4-106">Račun koji koristite za pokretanje simuliranih napada zahtijeva globalne dozvole za administratore ili bezbednosne administratore te multi-Factor provjeru autentičnosti (MFA).</span><span class="sxs-lookup"><span data-stu-id="b9cc4-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="b9cc4-107">Dodatne informacije o preduvjetima za simulator napada potražite u [ovoj temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="b9cc4-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="b9cc4-108">Važne informacije o **brutalnosti napada lozinka** za napade:</span><span class="sxs-lookup"><span data-stu-id="b9cc4-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="b9cc4-109">Ako je ciljni račun omogućen za MFA, a lozinka je ispravno pogađala, račun se neće prikazati kao kompromitiran (drugi faktor provjere autentičnosti bit će nepotpun).</span><span class="sxs-lookup"><span data-stu-id="b9cc4-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="b9cc4-110">Datoteka lozinke ne može biti veća od 10 MB.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="b9cc4-111">Koristite jednu lozinku po retku i uvrstite prazni redak (povrat u prijevozu) nakon posljednje lozinke na popisu.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="b9cc4-112">Važne informacije koje se odnose na **krađu identiteta** priložite simulacije:</span><span class="sxs-lookup"><span data-stu-id="b9cc4-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="b9cc4-113">Prema dizajnu ne možete pružiti prilagođenu vrijednost za **URL poslužitelja za prijavu krađe identiteta**.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="b9cc4-114">Ako primatelj koristi dodatak za [poruku izvješća](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) da bi prijavio poruku kao krađu identiteta, možda nećete primati upozorenja za poruku (jer je to simulirani napad).</span><span class="sxs-lookup"><span data-stu-id="b9cc4-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="b9cc4-115">Izvješća: nakon dovršetka simuliranog napada možete kliknuti **Detalji o napadu** da biste vidjeli izvješće.</span><span class="sxs-lookup"><span data-stu-id="b9cc4-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="b9cc4-116">Detaljne upute i nove značajke u simulatoru Attack potražite [u članku simulator napada u programu Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="b9cc4-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
