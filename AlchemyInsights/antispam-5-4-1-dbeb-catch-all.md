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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Rješavanje problema s isporučenjem za kôd pogreške 550 je odbijen pristup za prijenos

Taj se problem pojavljuje kada [Provjerite je li adresa e-pošte valjana da biste spriječili bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) prilikom ulaska u Microsoftovu mrežu. Pokušajte sljedeće:

1. Određivanje je li problem specifičan za cijelu domenu ili jednu adresu e-pošte:
    - Cijela domena: ponekad se domena mora sinkronizirati; Pokušajte [postaviti domenu na interno, a zatim natrag na autoritativno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna adresa e-pošte: ponekad adresa mora biti sinkronizirana; promjenom SMTP Proxy adrese, a zatim promjenom natrag, može pomoći.
2. Određivanje je li problem specifičan za grupu ili javnu mapu. Za neke vrste objekata objekti će se možda morati ručno stvoriti u servisu Azure Active Directory.

Ako vam je potrebna dodatna pomoć, otvorite karticu za podršku i navedite djelokrug problema (uključujući vrstu objekta koji šaljete) da bismo vam mogli bolje pomoći.