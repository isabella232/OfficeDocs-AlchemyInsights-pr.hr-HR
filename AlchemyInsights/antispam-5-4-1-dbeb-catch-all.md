---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821439"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="1e4f4-102">Rješavanje problema s isporukom za kod pogreške 550 5.4.1 Relay Access Denied</span><span class="sxs-lookup"><span data-stu-id="1e4f4-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="1e4f4-103">Taj se problem pojavljuje kada [provjeravate je li adresa e-pošte valjana da biste spriječili odskakanja prilikom](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ulaska u Microsoftovu mrežu.</span><span class="sxs-lookup"><span data-stu-id="1e4f4-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="1e4f4-104">Pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="1e4f4-104">Try the following:</span></span>

1. <span data-ttu-id="1e4f4-105">Odredite je li problem specifičan za cijelu domenu ili jednu adresu e-pošte:</span><span class="sxs-lookup"><span data-stu-id="1e4f4-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="1e4f4-106">Cijela domena: ponekad je potrebno sinkronizirati domenu; pokušajte [postaviti domenu na Interno, a zatim se vratiti na Mjerodavno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="1e4f4-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="1e4f4-107">Jedna adresa e-pošte: ponekad je potrebno sinkronizirati s adresom; promjena smtp proxy adrese, a zatim promjena povratka može vam pomoći.</span><span class="sxs-lookup"><span data-stu-id="1e4f4-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="1e4f4-108">Odredite je li problem specifičan za grupu ili javnu mapu.</span><span class="sxs-lookup"><span data-stu-id="1e4f4-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="1e4f4-109">Za neke vrste objekata objekti će se možda morati ručno stvoriti na servisu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1e4f4-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="1e4f4-110">Ako vam je potrebna dodatna pomoć, otvorite kartu za podršku i navedite opseg problema (uključujući vrstu objekta na koji šaljete) da bismo vam mogli bolje pomoći.</span><span class="sxs-lookup"><span data-stu-id="1e4f4-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>