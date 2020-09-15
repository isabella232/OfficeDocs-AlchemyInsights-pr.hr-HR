---
title: AntiSpam
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717353"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="a9669-102">Rješavanje problema s isporučenjem za kôd pogreške 550 je odbijen pristup za prijenos</span><span class="sxs-lookup"><span data-stu-id="a9669-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="a9669-103">Taj se problem pojavljuje kada [Provjerite je li adresa e-pošte valjana da biste spriječili bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) prilikom ulaska u Microsoftovu mrežu.</span><span class="sxs-lookup"><span data-stu-id="a9669-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="a9669-104">Pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="a9669-104">Try the following:</span></span>

1. <span data-ttu-id="a9669-105">Određivanje je li problem specifičan za cijelu domenu ili jednu adresu e-pošte:</span><span class="sxs-lookup"><span data-stu-id="a9669-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="a9669-106">Cijela domena: ponekad se domena mora sinkronizirati; Pokušajte [postaviti domenu na interno, a zatim natrag na autoritativno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="a9669-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="a9669-107">Jedna adresa e-pošte: ponekad adresa mora biti sinkronizirana; promjenom SMTP Proxy adrese, a zatim promjenom natrag, može pomoći.</span><span class="sxs-lookup"><span data-stu-id="a9669-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="a9669-108">Određivanje je li problem specifičan za grupu ili javnu mapu.</span><span class="sxs-lookup"><span data-stu-id="a9669-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="a9669-109">Za neke vrste objekata objekti će se možda morati ručno stvoriti u servisu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a9669-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="a9669-110">Ako vam je potrebna dodatna pomoć, otvorite karticu za podršku i navedite djelokrug problema (uključujući vrstu objekta koji šaljete) da bismo vam mogli bolje pomoći.</span><span class="sxs-lookup"><span data-stu-id="a9669-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>