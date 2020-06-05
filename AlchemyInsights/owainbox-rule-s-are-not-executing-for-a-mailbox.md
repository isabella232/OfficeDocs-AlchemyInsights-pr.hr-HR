---
title: 1332 OWA – pravila ulazne pošte ne izvršavaju se za poštanski sandučić
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576552"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravilo ulazne pošte ne funkcionira prema očekivanjima

Provjerite sljedeće postavke u programu Outlook na webu:

- Poruka se može preusmjeriti, proslijediti ili odgovoriti na automatsko na temelju pravila ulazne pošte samo jednom. Pravilo preusmjeravanja (pravilo ulazne pošte ili pravilo tijeka pošte, poznato i kao pravilo prijenosa) može dodati poruku najviše deset primatelja prosljeđivanja. Dodatne informacije potražite [u odjeljku Ograničenja pravila dnevnika, prijevoza i ulazne pošte](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Pravila ulazne pošte ne funkcioniraju na zamjenskom poštanskom sandučiću za dnevnike. Dodatne informacije o zamjenskom poštanskom sandučiću za dnevnike [potražite u odjeljku Zamjenski poštanski sandučić za dnevnike](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Da biste riješili te probleme, pogledajte [KB 2829319](https://support.microsoft.com/kb/2829319).

Ako se prethodni problemi ne primjenjuju, pokrenite dijagnostičko izvješće o pravilu mape Primljeno prije nego što eskalirati problem na Microsoftovu podršku:

1. Otvorite poštanski sandučić u programu Outlook na webu, a zatim kliknite <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Postavke i postavke**  >  **Prikaz svih postavki**  >  programa Outlook **Pošta**  >  **Pravila.**

2. Pri dnu stranice kliknite **Ako vaša pravila ne funkcioniraju, kliknite ovdje da biste generirali dijagnostičko izvješće**.
