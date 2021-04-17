---
title: Potrebna vam je pomoć s ograničenjima slanja e-pošte?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836271"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="a9306-102">Potrebna vam je pomoć s ograničenjima slanja e-pošte?</span><span class="sxs-lookup"><span data-stu-id="a9306-102">Need help with email sending limits?</span></span>

<span data-ttu-id="a9306-103">U nastavku se primjenjuju ograničenja slanja po **dizajnu** u servisu.</span><span class="sxs-lookup"><span data-stu-id="a9306-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="a9306-104">Dodatne informacije o tim ograničenjima dokumentirane su [ovdje](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="a9306-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="a9306-105">Da bismo obeshrabrili isporuku neželjenih masovnih poruka, primjenjujemo ograničenja stopa primatelja po korisniku na **sve odlazne i interne poruke.**</span><span class="sxs-lookup"><span data-stu-id="a9306-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="a9306-106">U svim SKU-ima to ograničenje **iznosi 10 000 primatelja dnevno.**</span><span class="sxs-lookup"><span data-stu-id="a9306-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="a9306-107">Korisnici koji moraju poslati legitimnu masovnu komercijalnu e-poštu (npr. biltene klijenata) trebali bi koristiti davatelje usluga drugih proizvođača koji su specijalizirani za te usluge.</span><span class="sxs-lookup"><span data-stu-id="a9306-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="a9306-108">**Napomena:** kada se dosegne ograničenje broja primatelja, poruke se ne mogu slati iz poštanskog sandučića dok broj primatelja koji su poslane poruke u protekla 24 sata ne padne ispod ograničenja.</span><span class="sxs-lookup"><span data-stu-id="a9306-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="a9306-109">Korisnik neće moći slati poruke do te točke.</span><span class="sxs-lookup"><span data-stu-id="a9306-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="a9306-110">Ograničenje brzine poruke **od 30 poruka po minuti primjenjuje se** na sve SKU-ove.</span><span class="sxs-lookup"><span data-stu-id="a9306-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="a9306-111">Time se određuje koliko poruka korisnik može poslati s računa za Exchange Online u određenom razdoblju.</span><span class="sxs-lookup"><span data-stu-id="a9306-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="a9306-112">Maksimalan broj primatelja dopuštenih u poljima **Prima, Kopija** i Skrivena kopija za jednu poruku e-pošte u svim SKU-ima **jest 1000 primatelja.**</span><span class="sxs-lookup"><span data-stu-id="a9306-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="a9306-113">Da biste prilagodili to ograničenje, [idite ovdje](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="a9306-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
