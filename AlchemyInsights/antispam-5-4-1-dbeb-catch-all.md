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
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964087"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Ispravite probleme isporuke za kod pogreške 550 5.4.1 pristup relej odbijen

Taj se problem pojavljuje prilikom [provjere da li je adresa e-pošte valjana kako bi se spriječilo izbacivanje](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) prilikom ulaska u mrežu Office 365. Pokušajte sljedeće:

1. Odredite je li problem specifičan za cijelu domenu ili jednu adresu e-pošte:
    - Cijela domena: ponekad je potrebno sinkronizirati domenu; Pokušajte [postaviti domenu na interno, a zatim natrag u autoritativno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
     - Jedna adresa e-pošte: ponekad je potrebno sinkronizirati adresu; promjenu SMTP adrese proxyja, a zatim ponovno mijenjanje može pomoći.
2. Odredite je li problem specifičan za grupu ili javnu mapu. Za neke vrste objekata, objekti možda moraju biti ručno stvoreni u Azure Active Directory.

Ako vam je potrebna dodatna pomoć, otvorite karticu za podršku i odredite opseg problema (uključujući vrstu objekta kojem šaljete) kako bismo vam mogli bolje pomoći.