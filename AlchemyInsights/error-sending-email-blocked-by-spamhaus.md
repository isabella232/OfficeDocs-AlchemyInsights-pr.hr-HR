---
title: Pogreška prilikom slanja e-pošte koju je blokirao SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946703"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Pogreška prilikom slanja e-pošte: glavno računalo klijenta je blokirano pomoću aplikacije Spamhaus

IP adresa koja je poslala poruku nalazi se na popisu blokiranih adresa u vlasništvu tvrtke [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Razlozi blokiranja servisa Spamhaus obuhvaćaju ugrožene račune, ugrožena računala koja zajednički dijele javnu IP adresu i pravilnike davatelja internetskih usluga (ISP-a). Mogući popravci su:
  
- Za blokirane dolazne poruke na kojima upravljate izvornim poslužiteljem e-pošte morate utvrditi uzrok i ukloniti blok s web-mjesta Servisa Spamhaus.

- Za blokirane dolazne poruke u kojima izvorna IP adresa pripada nekome drugome vlasnik adrese mora ukloniti blok s web-mjesta Spamhaus. Ako se IP adresa nalazi na popisu blokiranih pravilnika (PBL), vlasnik može dodijeliti drugu statičnu IP adresu ili ukloniti adresu iz PBL-a.

- Za blokirane odlazne poruke s vaše domene povezane s Microsoftom, tu pogrešku možete primiti ako se poruke usmjeravaju putem servisa treće strane. Da biste pronašli blokiranog vlasnika IP adrese, pomoću alata za pretraživanje WHOIS-a možete pronaći blokiranog vlasnika IP adrese.
