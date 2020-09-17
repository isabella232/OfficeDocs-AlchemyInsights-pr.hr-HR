---
title: Pogreška prilikom slanja e-pošte koju je blokirao SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783795"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Pogreška prilikom slanja e-pošte: klijentsko glavno računalo blokirano pomoću spamhaus

IP adresa koja je poslala poruku nalazi se na popisu blokova u vlasništvu servisa [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Razlozi zbog kojih je spamhaus blokirao obuhvaćaju ugroћene račune, kompromitirani strojevi koji zajednički koriste javnu IP adresu i pravila davatelja internetskih usluga (ISP-a). Mogući su popravci:
  
- Da biste blokirali ulazne poruke na kojima kontrolirate izvorni poslužitelj e-pošte, morate odrediti uzrok i ukloniti blok s web-mjesta spamhaus.

- Da biste blokirali ulazne poruke u kojima adresa izvornog IP-a pripada nekome drugome, vlasnik adrese mora ukloniti blok s web-mjesta spamhaus. Ako je IP adresa na popisu poljski blok (PBL), vlasnik može dodijeliti neku drugu statičnu IP adresu ili ukloniti adresu iz PBL-a.

- Ako ste blokirali odlazne poruke iz domene povezane s Microsoftom, možete primiti ovu pogrešku ako su poruke preusmjerene putem servisa trećih strana. Možete koristiti alat za traženje funkcije WHOIS da biste pronašli vlasnika blokiranih IP adresa.
