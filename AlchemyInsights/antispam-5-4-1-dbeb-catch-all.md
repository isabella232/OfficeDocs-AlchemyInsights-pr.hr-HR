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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Ispravite probleme isporuke za kod pogreške 550 5.4.1 pristup relej odbijen

Taj se problem pojavljuje prilikom [provjere da li je adresa e-pošte valjana kako bi se spriječilo izbacivanje](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) prilikom ulaska u mrežu Office 365. Pokušajte sljedeće:

1. Odredite je li problem specifičan za cijelu domenu ili jednu adresu e-pošte:
    - Cijela domena: ponekad je potrebno sinkronizirati domenu; Pokušajte [postaviti domenu na interno, a zatim natrag u autoritativno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna adresa e-pošte: ponekad je potrebno sinkronizirati adresu; promjenu SMTP adrese proxyja, a zatim ponovno mijenjanje može pomoći.
2. Odredite je li problem specifičan za grupu ili javnu mapu. Za neke vrste objekata, objekti možda moraju biti ručno stvoreni u Azure Active Directory.

Ako vam je potrebna dodatna pomoć, otvorite karticu za podršku i odredite opseg problema (uključujući vrstu objekta kojem šaljete) kako bismo vam mogli bolje pomoći.