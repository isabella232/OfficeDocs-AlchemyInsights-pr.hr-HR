---
title: Zaštita od napada na Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035077"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="d6484-102">Zaštita od napada na Backscatter</span><span class="sxs-lookup"><span data-stu-id="d6484-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="d6484-103">Backscatter je izvješće o neisporuci (koje se nazivaju i poruke NDRs ili Bounce) koje primate za poruke koje niste slali.</span><span class="sxs-lookup"><span data-stu-id="d6484-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="d6484-104">Spameri Forge (podvala) **iz:** adresa svojih poruka, a često koriste i stvarne adrese e-pošte da bi mogli prenijeti vjerodostojnost porukama.</span><span class="sxs-lookup"><span data-stu-id="d6484-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="d6484-105">Dakle, kada spameri neminovno pošalju poruke nepostojećim primateljima, odredišni poslužitelj e-pošte u suštini je prevaren da vrati neisporučenu poruku u NDR u falsificirani pošiljatelj iz **:** adresa.</span><span class="sxs-lookup"><span data-stu-id="d6484-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="d6484-106">Dodatne informacije možete pronaći u odjeljku [Backscatter u programu eeiop](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="d6484-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="d6484-107">**Omogućavanje zaštite Pozadinnog raspršivanja**</span><span class="sxs-lookup"><span data-stu-id="d6484-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="d6484-108">Da biste omogućili zaštitu od povratnog raspršivanja, slijedite put u nastavku.</span><span class="sxs-lookup"><span data-stu-id="d6484-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="d6484-109">**Protection.Office.com > upravljanje prijetnjama > Policy > antispam > odaberite pravilnik o filtriranju neželjene pošte i uređivanje pravilnika > svojstva neželjene pošte > označiti kao neželjena pošta > NDR odzivu > postavite ga na "uključeno"**</span><span class="sxs-lookup"><span data-stu-id="d6484-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="d6484-110">Ako smatrate da je račun ugrožen, pročitajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="d6484-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="d6484-111">Odgovaranje na kompromitirani račun e-pošte</span><span class="sxs-lookup"><span data-stu-id="d6484-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="d6484-112">Uklanjanje blokiranih korisnika s portala ograničenog korisnika u sustavu Office 365</span><span class="sxs-lookup"><span data-stu-id="d6484-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



