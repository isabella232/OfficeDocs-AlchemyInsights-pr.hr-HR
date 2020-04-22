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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Rješavanje problema s isporukom za šifru pogreške 550 5.4.1 Pristup releju je odbijen

Taj se problem pojavljuje [prilikom provjere je li adresa e-pošte valjana da biste spriječili povrat e-pošte](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) prilikom unosa Microsoftove mreže. Pokušajte sljedeće:

1. Odredite je li problem specifičan za cijelu domenu ili jednu adresu e-pošte:
    - Cijela domena: ponekad je potrebno sinkronizirati domenu; pokušajte [postaviti domenu na Interno, a zatim se vratite na mjerodavno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna adresa e-pošte: ponekad se adresa mora sinkronizirati; mjenjanje smtp proksiji adresa i tada mjenjanje Internet leđa može pomoć.
2. Odredite je li problem specifičan za grupu ili javnu mapu. Za neke vrste objekata objekte će možda morati ručno stvoriti u servisu Azure Active Directory.

Ako vam je potrebna dodatna pomoć, otvorite ulaznicu za podršku i navedite opseg problema (uključujući vrstu objekta na koji šaljete) kako bismo vam mogli pomoći bolje.