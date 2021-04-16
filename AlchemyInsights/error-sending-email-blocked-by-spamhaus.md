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
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813716"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Pogreška prilikom slanja e-pošte: glavno računalo klijenta je blokirano pomoću aplikacije Spamhaus

IP adresa koja je poslala poruku nalazi se na popisu blokiranih adresa u vlasništvu tvrtke [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Razlozi blokiranja servisa Spamhaus obuhvaćaju ugrožene račune, ugrožena računala koja zajednički dijele javnu IP adresu i pravilnike davatelja internetskih usluga (ISP-a). Mogući popravci su:
  
- Za blokirane dolazne poruke na kojima upravljate izvornim poslužiteljem e-pošte morate utvrditi uzrok i ukloniti blok s web-mjesta Servisa Spamhaus.

- Za blokirane dolazne poruke u kojima izvorna IP adresa pripada nekome drugome vlasnik adrese mora ukloniti blok s web-mjesta Spamhaus. Ako se IP adresa nalazi na popisu blokiranih pravilnika (PBL), vlasnik može dodijeliti drugu statičnu IP adresu ili ukloniti adresu iz PBL-a.

- Za blokirane odlazne poruke s vaše domene povezane s Microsoftom, tu pogrešku možete primiti ako se poruke usmjeravaju putem servisa treće strane. Da biste pronašli blokiranog vlasnika IP adrese, pomoću alata za pretraživanje WHOIS-a možete pronaći blokiranog vlasnika IP adrese.
