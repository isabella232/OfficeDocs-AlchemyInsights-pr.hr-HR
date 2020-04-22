---
title: AntiSpam 5.4.1 DBEB catch-all
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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707903"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="55a09-102">Rješavanje problema s isporukom za šifru pogreške 550 5.4.1 Pristup releju je odbijen</span><span class="sxs-lookup"><span data-stu-id="55a09-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="55a09-103">Taj se problem pojavljuje [prilikom provjere je li adresa e-pošte valjana da biste spriječili povrat e-pošte](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) prilikom unosa Microsoftove mreže.</span><span class="sxs-lookup"><span data-stu-id="55a09-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="55a09-104">Pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="55a09-104">Try the following:</span></span>

1. <span data-ttu-id="55a09-105">Odredite je li problem specifičan za cijelu domenu ili jednu adresu e-pošte:</span><span class="sxs-lookup"><span data-stu-id="55a09-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="55a09-106">Cijela domena: ponekad je potrebno sinkronizirati domenu; pokušajte [postaviti domenu na Interno, a zatim se vratite na mjerodavno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="55a09-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="55a09-107">Jedna adresa e-pošte: ponekad se adresa mora sinkronizirati; mjenjanje smtp proksiji adresa i tada mjenjanje Internet leđa može pomoć.</span><span class="sxs-lookup"><span data-stu-id="55a09-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="55a09-108">Odredite je li problem specifičan za grupu ili javnu mapu.</span><span class="sxs-lookup"><span data-stu-id="55a09-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="55a09-109">Za neke vrste objekata objekte će možda morati ručno stvoriti u servisu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="55a09-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="55a09-110">Ako vam je potrebna dodatna pomoć, otvorite ulaznicu za podršku i navedite opseg problema (uključujući vrstu objekta na koji šaljete) kako bismo vam mogli pomoći bolje.</span><span class="sxs-lookup"><span data-stu-id="55a09-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>