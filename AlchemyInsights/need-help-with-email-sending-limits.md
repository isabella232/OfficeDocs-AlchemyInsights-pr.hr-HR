---
title: Potrebna vam je pomoć s ograničenjima slanja e-pošte?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702355"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="75600-102">Potrebna vam je pomoć s ograničenjima slanja e-pošte?</span><span class="sxs-lookup"><span data-stu-id="75600-102">Need help with email sending limits?</span></span>

<span data-ttu-id="75600-103">U nastavku je **ograničeno slanje ograničenja** koja se primjenjuju u servisu.</span><span class="sxs-lookup"><span data-stu-id="75600-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="75600-104">Dodatne informacije o ovim ograničenjima dokumentirano je [ovdje](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="75600-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="75600-105">Da biste obeshrabruli isporuku neželjenih skupnih poruka, primjenjuju **se ograničenja stope primatelja po korisniku na sve izlazne i interne poruke**.</span><span class="sxs-lookup"><span data-stu-id="75600-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="75600-106">U cijelom skusu to ograničenje iznosi **10.000 primatelja po danu**.</span><span class="sxs-lookup"><span data-stu-id="75600-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="75600-107">Korisnici koji moraju slati legitimne komercijalne poruke e-pošte (na primjer, kupci Newsletteri) trebali bi koristiti treće strane koje su specijalizirane za te servise.</span><span class="sxs-lookup"><span data-stu-id="75600-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="75600-108">**Pažnja**: kada se dosegne ograničenje stope primatelja, poruke se ne mogu slati iz poštanskog sandučića dok broj primatelja koji su poslane poruke u zadnjih 24 sata ne padne ispod ograničenja.</span><span class="sxs-lookup"><span data-stu-id="75600-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="75600-109">Korisnik neće moći prenijeti poruke do te točke.</span><span class="sxs-lookup"><span data-stu-id="75600-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="75600-110">Ograničenje stope poruke od **30 poruka po minuti** primjenjuje se u cijelom skusu.</span><span class="sxs-lookup"><span data-stu-id="75600-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="75600-111">Time se određuje koliko poruka korisnik može putem računa sustava Exchange Online uputiti u određeno razdoblje.</span><span class="sxs-lookup"><span data-stu-id="75600-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="75600-112">**Maksimalan broj primatelja koji su dopušteni u poljima Prima, kopija i Skrivena kopija** za jednu poruku e-pošte, na svim SKUs-u, predstavlja **1000 primatelja**.</span><span class="sxs-lookup"><span data-stu-id="75600-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="75600-113">Da biste prilagodili ovo ograničenje, idite [ovdje](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="75600-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
