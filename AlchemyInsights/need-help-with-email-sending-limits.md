---
title: Potrebna vam je pomoć s ograničenjima slanja e-pošte?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357397"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="d5140-102">Potrebna vam je pomoć s ograničenjima slanja e-pošte?</span><span class="sxs-lookup"><span data-stu-id="d5140-102">Need help with email sending limits?</span></span>

<span data-ttu-id="d5140-103">U nastavku su **ograničenja slanja po dizajnu** koja se provode u usluzi.</span><span class="sxs-lookup"><span data-stu-id="d5140-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="d5140-104">Više informacija o tim ograničenjima dokumentirano je [ovdje](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="d5140-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="d5140-105">Da bismo obeshrabrili isporuku neželjenih masovnih poruka, primjenjujemo **ograničenja stope primatelja po korisniku na sve izlazne i interne poruke**.</span><span class="sxs-lookup"><span data-stu-id="d5140-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="d5140-106">U svim SkU-ovima, to ograničenje je **10.000 primatelja dnevno.**</span><span class="sxs-lookup"><span data-stu-id="d5140-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="d5140-107">Korisnici koji trebaju poslati legitimnu masovnu komercijalnu e-poštu (na primjer, biltene klijenata) trebali bi koristiti davatelje usluga trećih strana koji se specijaliziraju za te usluge.</span><span class="sxs-lookup"><span data-stu-id="d5140-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="d5140-108">**Napomena:** Nakon što se dosegne ograničenje broja primatelja, poruke se ne mogu slati iz poštanskog sandučića dok broj primatelja koji su poslani poruke u posljednja 24 sata padne ispod ograničenja.</span><span class="sxs-lookup"><span data-stu-id="d5140-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="d5140-109">Korisnik neće moći slati poruke do tog trenutka.</span><span class="sxs-lookup"><span data-stu-id="d5140-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="d5140-110">Ograničenje brzine slanja od **30 poruka u minuti** primjenjuje se u svim JSK-ovima.</span><span class="sxs-lookup"><span data-stu-id="d5140-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="d5140-111">Time se određuje koliko poruka korisnik može poslati s a svojim računom sustava Exchange Online u određenom razdoblju.</span><span class="sxs-lookup"><span data-stu-id="d5140-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="d5140-112">**Maksimalan broj primatelja dopuštenih u poljima Prima, Kopija i Skrivena kopija** za jednu poruku e-pošte u svim JSK-ovima je **1000 primatelja**.</span><span class="sxs-lookup"><span data-stu-id="d5140-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="d5140-113">Da biste prilagodili to ograničenje, idite [ovdje](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="d5140-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
