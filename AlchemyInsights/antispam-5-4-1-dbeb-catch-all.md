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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Rješavanje problema s isporukom za kod pogreške 550 5.4.1 Relay Access Denied

Taj se problem pojavljuje kada [provjeravate je li adresa e-pošte valjana da biste spriječili odskakanja prilikom](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ulaska u Microsoftovu mrežu. Pokušajte sljedeće:

1. Odredite je li problem specifičan za cijelu domenu ili jednu adresu e-pošte:
    - Cijela domena: ponekad je potrebno sinkronizirati domenu; pokušajte [postaviti domenu na Interno, a zatim se vratiti na Mjerodavno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna adresa e-pošte: ponekad je potrebno sinkronizirati s adresom; promjena smtp proxy adrese, a zatim promjena povratka može vam pomoći.
2. Odredite je li problem specifičan za grupu ili javnu mapu. Za neke vrste objekata objekti će se možda morati ručno stvoriti na servisu Azure Active Directory.

Ako vam je potrebna dodatna pomoć, otvorite kartu za podršku i navedite opseg problema (uključujući vrstu objekta na koji šaljete) da bismo vam mogli bolje pomoći.