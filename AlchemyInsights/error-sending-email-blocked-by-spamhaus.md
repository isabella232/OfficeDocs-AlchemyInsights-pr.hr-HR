---
title: Pogreška pri slanju e-pošte koju je blokirao SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714250"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Pogreška pri slanju e-pošte: Glavno računalo klijenta blokirano je pomoću usluge Spamhaus

IP adresa koja je poslala poruku nalazi se na popisu blokova u vlasništvu [Spamhausa](https://go.microsoft.com/fwlink/p/?linkid=123245). Razlozi za blokiranje u spamhausu uključuju ugrožene račune, kompromitirane strojeve koji dijele javnu IP adresu i pravila davatelja internetskih usluga (ISP- a). Mogući popravci su:
  
- Za blokirane dolazne poruke u kojima upravljate izvornim poslužiteljem e-pošte morate odrediti uzrok i ukloniti blok s web-mjesta Spamhaus.

- Za blokirane dolazne poruke gdje izvorNA IP adresa pripada nekome drugome, vlasnik adrese mora ukloniti blok s web-mjesta Spamhaus. Ako se IP adresa nalazi na popisu blokiranih pravila (PBL), vlasnik može dodijeliti drugu statičku IP adresu ili ukloniti adresu iz PBL-a.

- Za blokirane izlazne poruke s domene povezane s Microsoftom možete primiti ovu pogrešku ako se poruke usmjeravaju putem servisa treće strane. Pomoću whois alata za pretraživanje možete pronaći vlasnika blokirane IP adrese.
