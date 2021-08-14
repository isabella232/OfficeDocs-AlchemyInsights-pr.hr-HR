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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932269"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Rješavanje problema s isporukom za kod pogreške 550 5.4.1 Relay Access Denied

Taj se problem pojavljuje kada [provjeravate je li adresa e-pošte valjana da biste spriječili odskakanja prilikom](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ulaska u Microsoftovu mrežu. Pokušajte sljedeće:

1. Odredite je li problem specifičan za cijelu domenu ili jednu adresu e-pošte:
    - Cijela domena: ponekad je potrebno sinkronizirati domenu; pokušajte [postaviti domenu na Interno, a zatim se vratiti na Mjerodavno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna adresa e-pošte: ponekad je potrebno sinkronizirati s adresom; promjena smtp proxy adrese, a zatim promjena povratka može vam pomoći.
2. Odredite je li problem specifičan za grupu ili javnu mapu. Za neke vrste objekata objekti će se možda morati ručno stvoriti u Azure Active Directory.

Ako vam je potrebna dodatna pomoć, otvorite kartu za podršku i navedite opseg problema (uključujući vrstu objekta na koji šaljete) da bismo vam mogli bolje pomoći.