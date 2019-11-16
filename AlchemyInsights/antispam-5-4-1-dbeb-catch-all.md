---
title: AntiSpam 5.4.1 DBEB Catch-sve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672425"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="cef34-102">Ispravite probleme isporuke za kod pogreške 550 5.4.1 pristup relej odbijen</span><span class="sxs-lookup"><span data-stu-id="cef34-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="cef34-103">Taj se problem pojavljuje prilikom [provjere da li je adresa e-pošte valjana kako bi se spriječilo izbacivanje](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) prilikom ulaska u mrežu Office 365.</span><span class="sxs-lookup"><span data-stu-id="cef34-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="cef34-104">Pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="cef34-104">Try the following:</span></span>

1. <span data-ttu-id="cef34-105">Odredite je li problem specifičan za cijelu domenu ili jednu adresu e-pošte:</span><span class="sxs-lookup"><span data-stu-id="cef34-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="cef34-106">Cijela domena: ponekad je potrebno sinkronizirati domenu; Pokušajte [postaviti domenu na interno, a zatim natrag u autoritativno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="cef34-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="cef34-107">Jedna adresa e-pošte: ponekad je potrebno sinkronizirati adresu; promjenu SMTP adrese proxyja, a zatim ponovno mijenjanje može pomoći.</span><span class="sxs-lookup"><span data-stu-id="cef34-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="cef34-108">Odredite je li problem specifičan za grupu ili javnu mapu.</span><span class="sxs-lookup"><span data-stu-id="cef34-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="cef34-109">Za neke vrste objekata, objekti možda moraju biti ručno stvoreni u Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cef34-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="cef34-110">Ako vam je potrebna dodatna pomoć, otvorite karticu za podršku i odredite opseg problema (uključujući vrstu objekta kojem šaljete) kako bismo vam mogli bolje pomoći.</span><span class="sxs-lookup"><span data-stu-id="cef34-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>